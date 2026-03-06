**Notes from conversations - the info on this page needs verifying**

***

From https://ibm-cloud.slack.com/archives/C30NGTBFS/p1753978393359689 (internal)

Liberty does not support looking up EJBs remotely using the `java:global` name.  Instead, remote lookups must use the corbaname, so the lookup string must look like this: ```corbaname::test.ibm.com:2809#ejb/global/ExampleApp/ExampleModule/ExampleHomeBean!com.ibm.example.ExampleEJBHome corbaname:rir:#ejb/global/ExampleApp/ExampleModule/ExampleHomeBean!com.ibm.example.ExampleEJBHome```. `providerUrl` needs to be of the format `corbaname::<hostname>:<hostport>`. Then, to convert from the `java:global` name to the corbaname, you replace `java:` with `ejb/`. Depending on your interface, if it only contains a single "." character, then you will also need to escape the ".". More details and examples of using the corbanmae, including escaping may be found here: [Using enterprise JavaBeans with remote interfaces on Liberty](https://www.ibm.com/docs/en/was-liberty/core?topic=liberty-using-enterprise-javabeans-remote-interfaces)


***

From https://ibm-cloud.slack.com/archives/C30NGTBFS/p1753257291151479 (internal)

A liberty server hosting an EJB only makes that EJB available to remote processes via the CORBA name service with a name like:
`corbaname::localhost:2809#ejb/global/ProjectEJBEAR-0.0.1-SNAPSHOT/ProjectEJB/ExampleEJB!com.client.example.IExampleEJB`

However, there are a couple of options for adding configuration to the client side to achieve something close to what is requested.

## Option 1 - add an EJB reference to the client application.

For example, if they add something like this to the client side web.xml or application.xml file:
```
<ejb-ref>
    <ejb-ref-name>java:global/com.client.example.IExampleEJB</ejb-ref-name>
    <ejb-ref-type>Session</ejb-ref-type>
    <remote>com.ibm.svt.populateModule.grade.PriceSession</remote>
</ejb-ref>
```

Then add a mapping in either `ibm-web-bnd.xml` , or `ibm-application-bnd.xml` or in the `webApplication` section of `server.xml`

```
  <ejb-ref name="java:global/com.client.example.IExampleEJB" binding-name="corbaname::localhost:2809#ejb/global/ProjectEJBEAR-0.0.1-SNAPSHOT/ProjectEJB/ExampleEJB!com.client.example.IExampleEJB"/>
```

Then the client side code would look like this:
```
InitialContext ctx = new InitialContext();
Object obj = ctx.lookup("java:global/" + IExampleEJB.class.getName());
IExampleEJB ejb = (IExampleEJB)PortableRemoteObject.narrow(obj, IExampleEJB.class);
```

Very similar to what is being asked for, with just the addition of `java:global/` as a prefix to the interface name.
The EJB reference is effectively creating an alias on the client side, which is then re-directed to the EJB on the server side.  The reference would need to be added to the application itself, in either web.xml, application.xml or as an @EJB annotation on a servlet class, but the mapping to the real EJB can either be in a binding file in the application, or just directly in the server server.xml file.

## Option 2 - bind the real EJB string into JNDI with the desired name

Something like this could be added in server.xml:

```
  <jndiEntry jndiName="com.client.example.IExampleEJB" value="corbaname::localhost:2809#ejb/global/ProjectEJBEAR-0.0.1-SNAPSHOT/ProjectEJB/ExampleEJB!com.client.example.IExampleEJB" />
```

or even

```
   <jndiEntry jndiName="com.client.example.IExampleEJB" value="${ejb.IExampleEJB}" />
```

Where ${ejb.IExampleEJB} is an environment variable set to the real location

The then application code would look like this:

```
InitialContext ctx = new InitialContext();
String ejbJndiName = ctx.lookup(IExampleEJB.class.getName());
Object obj = ctx.lookup(ejbJndiName);
IExampleEJB ejb = (IExampleEJB)PortableRemoteObject.narrow(obj, IExampleEJB.class);
```

So, the application code would only need to use the interface name, but would require a second lookup based on the result.
These are a couple of options; there may be other options a swell, but the idea is to create some type of alias on the client side that is then mapped to the real name, such that the real name is removed from the application and easily adjustable.

Another option that may work, though I have not tried myself is to use <jndiObjectFactory> and <jndiReferenceEntry> to bind the EJB interface name to an ObjectFactory, where the ObjectFactory knows how to lookup the EJB.  This potentially may allow you to use only the EJB interface name in the application, but would require the overhead of implementing ObjectFactory(s).
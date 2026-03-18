This knowledge base provides a collection of links to information about how to migrate a WebSphere Application Server application to run on [Liberty](https://www.ibm.com/products/liberty).

The knowledge base is managed and curated by [Laura Cowen](https://github.com/lauracowen), Technical Content Strategist and Developer Advocate at IBM. Contributions and feedback are welcome from WebSphere users and subject matter experts.

For more info about the knowledge base aims and how to contribute, see the [README](https://github.com/WASdev/websphere-and-liberty).

To search for information, use your browser's search in page feature (CTRL+F).

If there is something missing, or you have information that would answer a question on the knowledge base, please [raise an issue](https://github.com/WASdev/websphere-and-liberty/issues/new).


# Liberty overview

* [WebSphere Liberty built on Open Liberty](https://www.ibm.com/docs/en/was-liberty/base?topic=liberty-overview) (WL docs)
* Economics of Liberty ([issue](https://github.com/WASdev/websphere-and-liberty/issues/26))
* Intro to Liberty from a tWAS perspective ([issue](https://github.com/WASdev/websphere-and-liberty/issues/27))
* Overview of various target platforms for apps and when to choose them (eg MoRE (Liberty with tWAS operations), Liberty on VM, Liberty in containers, etc) ([issue](https://github.com/WASdev/websphere-and-liberty/issues/28))
  * [MoRE](https://www.ibm.com/docs/en/more) (docs)
  * [EAR](https://www.ibm.com/docs/en/ear) (docs)
* Liberty downloads and licensing options and guidance ([issue](https://github.com/WASdev/websphere-and-liberty/issues/29))
* [Liberty support for Java SE 8 until December 2030](https://community.ibm.com/community/user/blogs/macdara-butler/2025/11/13/liberty-java-8-support)

## Why Liberty

* [6 Reasons for WebSphere Liberty](https://developer.ibm.com/articles/6-reasons-why-open-liberty-is-an-ideal-choice-for-developing-and-deploying-microservices/) (IBM Developer)
* [Why cloud-native developers love Liberty](https://developer.ibm.com/articles/why-cloud-native-java-developers-love-liberty/) (IBM Developer)
* Operations:
  * [Effortless updates require a zero-migration policy](https://foojay.io/today/effortless-updates-zero-migration/) (article)
  * [Zero migration](https://openliberty.io/docs/latest/zero-migration-architecture.html) (OL docs)
  * [Achieve high performance Java applications with IBM Semeru Runtimes and Open Liberty](https://developer.ibm.com/articles/j-java-performance/)
* Developers:
  * [Five Java Developer Must-Haves for Ultra-Fast Startup Solutions](https://dzone.com/articles/five-java-developer-must-haves-for-ultra-fast-star) (article)
  * [Java Virtual Threads: A Case Study](https://www.infoq.com/articles/java-virtual-threads-a-case-study/) (article)
  * [Dev mode](https://openliberty.io/docs/latest/development-mode.html) (OL docs)
  * [Dev mode](https://youtu.be/QDLEr0mTwxM?si=hMhzBI6fIzi_Z751) (video)
  * [Easily enhance your modernized Java EE applications with Liberty and dev mode](https://youtu.be/XBW7RUdwb-0?si=EqCs8DYz-a1D7kdM) (video)
  * [Liberty Tools in Visual Studio Code](https://foojay.io/today/effective-cloud-native-development-open-liberty-vs-code/) (article)
  * [Developer Deep Dive of Liberty Tools for Visual Studio Code](https://youtu.be/TOfQi-C8AEU?si=BPCi9OG3Ip6hDQPS) (video; we also have several short snippets)
  * [Liberty Tools in Eclipse IDE (Foojay.io)](https://foojay.io/today/effective-cloud-native-development-eclipse-ide-open-liberty/) (article)
  * [Liberty Tools in IntelliJ IDE (Foojay.io)](https://foojay.io/today/effective-cloud-native-java-app-development-with-open-liberty-in-intellij-idea/) (article)
  * [Developer Deep Dive of Liberty Tools for IntelliJ IDEA](https://youtu.be/O-dN3yHSPdQ?si=3vB7YTgNlmlpDu2f) (video)
  * [Liberty developer guides](https://openliberty.io/guides/) (OL guides)

## Liberty architecture

* [Liberty capabilities (programming models and services) are organized into modular features](https://openliberty.io/docs/latest/reference/feature/feature-overview.html) (OL docs)
* [Liberty server configuration overview](https://openliberty.io/docs/latest/reference/config/server-configuration-overview.html) (OL docs)
* [Liberty directories and properties](https://openliberty.io/docs/latest/reference/directory-locations-properties.html) (OL docs)
* [Liberty architecture overview](https://www.ibm.com/docs/en/was-liberty/base?topic=overview-architecture) (WL docs)
* [Liberty architecture overview, p8-20](https://www.redbooks.ibm.com/redbooks/pdfs/sg248170.pdf) (RB Liberty admin)

## Liberty operations

* [Demystifying Liberty for WebSphere administrators](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/) (article with embedded videos)

Deployment options:

* Deploying Liberty servers on traditional VMs:
  * [Deploying Liberty servers in a tWAS environment with MoRE](https://community.ibm.com/community/user/viewdocument/enterprise-application-runtimes-a?CommunityKey=1348d157-c61b-417f-928a-179c3d0ffccb&tab=librarydocuments) (video)
  * [Cost-effective options for Java modernization](https://community.ibm.com/community/user/viewdocument/ear-and-ama-cost-effective-options?CommunityKey=1348d157-c61b-417f-928a-179c3d0ffccb&tab=librarydocuments) (video)
* Deploying Liberty servers in containers
  * [Cost-effective options for Java modernization](https://community.ibm.com/community/user/viewdocument/ear-and-ama-cost-effective-options?CommunityKey=1348d157-c61b-417f-928a-179c3d0ffccb&tab=librarydocuments) (video)


## Liberty application frameworks

* [WebSphere Liberty and Open Liberty table of features](https://ibm.ent.box.com/file/257278582790?v=LibertyPeriodicTable) (slides)
* [MicroProfile](https://openliberty.io/docs/latest/microprofile.html) (OL docs)
  * [MicroProfile version support](https://www.ibm.com/docs/en/was-liberty/base?topic=architecture-microprofile-programming-model-support) (WL docs)
* [Jakarta EE and Java SE](https://openliberty.io/docs/latest/jakarta-ee.html) (OL docs)
  * [Java SE support](https://openliberty.io/docs/latest/java-se.html) (OL docs)
  * [Jakarta EE 10 support](https://www.ibm.com/docs/en/was-liberty/base?topic=architecture-jakarta-ee-10-programming-model-support) (WL docs)
  * [Jakarta EE 9.1 support](https://www.ibm.com/docs/en/was-liberty/base?topic=architecture-jakarta-ee-91-programming-model-support) (WL docs)
  * [Jakarta EE 8 and Java EE 8 support](https://www.ibm.com/docs/en/was-liberty/base?topic=architecture-jakarta-java-ee-8-in-liberty) (WL docs)
  * [Java EE 7 support](https://www.ibm.com/docs/en/was-liberty/base?topic=liberty-java-ee-7-programming-model-support) (WL docs)
  * [Java EE 6 support](https://www.ibm.com/docs/en/was-liberty/base?topic=architecture-java-ee-6-programming-model-support) (WL docs)
  * [Spring Boot support](https://www.ibm.com/docs/en/was-liberty/base?topic=architecture-spring-boot-programming-model-support) (WL docs)
* [Liberty externals support](https://www.ibm.com/docs/en/was-liberty/base?topic=architecture-liberty-externals-support) (WL docs)

* [Liberty Tools for IDEs](https://openliberty.io/docs/latest/develop-liberty-tools.html) (OL docs)

# Differences between Liberty and WebSphere


(LC: Ultimately, I think this would be more useful to be framed in terms of goals, as "I do it this way on WebSphere; how should I do it on Liberty?", rather than highlighting the differences.)

## Architectural differences

* Overview of architectural differences between WebSphere and Liberty. ([issue](https://github.com/WASdev/websphere-and-liberty/issues/31)) Based on sources:
  * [Liberty architecture](#liberty-architecture)
  * [Liberty operations](#liberty-operations)
  * [Liberty applications support](#liberty-application-support)
  * [WebSphere architecture](https://www.ibm.com/docs/en/was/9.0.5?topic=websphere-application-server-overview)
  * [WebSphere architecture (admin redbook p3-28)](https://www.redbooks.ibm.com/redbooks/pdfs/sg248056.pdf)
  * [WebSphere architecture (migration redbook p8-17)](https://www.redbooks.ibm.com/redbooks/pdfs/sg248048.pdf)

## Operational differences

* [Demystifying Liberty for WebSphere administrators](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/) (article with embedded videos))

## Application framework differences

* Overview of application framework differences ([issue](https://github.com/WASdev/websphere-and-liberty/issues/33)) Cover the following topics at a high level:
  * Java SE versions
  * Java EE / Jakarta EE versions
  * [Remote transaction propagation between remote EJBs](https://community.ibm.com/community/user/blogs/laura-cowen1/2025/09/12/transaction-propagation-on-liberty)
  * ? Other things likely to be flagged by binary scanner?
  * Spring and Spring Boot on Liberty

(Provide links out to detailed instructions in later sections.)

# Getting to know Liberty



While tWAS applications are largely compatible with running on Liberty, Liberty is not identical to tWAS. Before you start to migrate a tWAS application to run on Liberty, it is worth becoming familiar with writing and running apps on Liberty. WebSphere Liberty is built on Open Liberty; apart from [a small number of additional capabilities in WebSphere Liberty](https://www.ibm.com/docs/en/was-liberty/nd?topic=liberty-overview), the WebSphere Liberty and Open Liberty runtimes are the same.

* Build a new app
  * [Getting started with Open Liberty](https://openliberty.io/guides/getting-started.html) (OL guide)
  * [Generate a start project](https://openliberty.io/start/) (OL tools)
  * [Building applications with Maven and Gradle](https://openliberty.io/guides/#build)
  * [Creating RESTful web service](https://openliberty.io/guides/rest-intro.html) (OL guide)
* Learning more about writing and deploying applications on Liberty
  * [Securing applications](https://openliberty.io/guides/#security) (OL guide)
  * [Accessing data from Liberty applications](https://openliberty.io/guides/#persistence) (OL guide)
  * [Test tools](https://openliberty.io/guides/#test) (OL guide)
  * [Containerizing applications on Liberty](https://openliberty.io/guides/#containerize) (OL guide)
  * [How to package your cloud-native Java application for rapid startup](https://openliberty.io/blog/2023/06/29/rapid-startup-instanton.html) (OL blog)

See [Other resources](#other-resources) for more help.

# Planning a migration

* [What is application modernization? (concepts on ibm.com)](https://www.ibm.com/think/topics/application-modernization)
* [Java Application Modernization Playbook](https://ibm.github.io/app-mod-journey/tree/index.html)
* [Tour of App Mod Playbook](https://www.youtube.com/watch?v=iyLrL-S0UjM) (video)
* [Getting started with application modernization](https://developer.ibm.com/learningpaths/get-started-application-modernization/) (IBM Developer; needs updating)
* [Modernizing applications to use WebSphere Liberty](https://developer.ibm.com/learningpaths/app-mod-liberty/) (IBM Developer; needs updating)
* [WebSphere Migration Knowledge Collection](https://www.ibm.com/support/pages/node/318851) (needs reviewing)
* [Migrating WebSphere Traditional Versions](https://www.ibm.com/support/pages/websphere-migration-knowledge-collection-migrating-websphere-traditional-versions) (needs reviewing/updating)
* [Migrating to Liberty](https://www.ibm.com/support/pages/node/318851) (needs reviewing/updating)
* [Migration info in WebSphere docs](https://www.ibm.com/docs/en/was-liberty/base?topic=migrating-applications-liberty) (docs)
* Scanning estate and choosing an application for migration, create migration plan ([issue](https://github.com/WASdev/websphere-and-liberty/issues/34))
* Follow migration plan in AMA (show examples or what it provides); "I've got the AMA bundle, what do I do with it?" ([issue](https://github.com/WASdev/websphere-and-liberty/issues/35))

## Tools to help you migrate to Liberty
  
* Tools to help you migrate to Liberty ([issue](https://github.com/WASdev/websphere-and-liberty/issues/9))
![Diagram showing the tools.](https://github.com/user-attachments/assets/59e63e66-fa22-4a8b-b3e7-a05788aa4187)
    * Application Modernization Accelerator (AMA)
      * [Application Modernization Accelerator documentation](https://www.ibm.com/docs/en/ama) (docs)
      * [AMA update and demo (Application Modernization Accelerator)](https://community.ibm.com/community/user/viewdocument/ama-update-and-demo-application-mo?CommunityKey=1348d157-c61b-417f-928a-179c3d0ffccb&tab=librarydocuments) (video)
    * AMA Dev tools
      * [Easily modernize Java applications in your IDE with AMA Dev Tools](https://developer.ibm.com/articles/modernize-java-applications-ama-dev-tools/)
  * Developer tools
    * Liberty Dev tools
      * [Effective cloud-native Java app development with Liberty in IntelliJ IDEA](https://developer.ibm.com/articles/awb-effective-cloud-native-development-open-liberty-intellij-idea)
      * [Effective cloud native development with Liberty in Visual Studio Code](https://developer.ibm.com/articles/awb-effective-cloud-native-development-open-liberty-vs-code)
      * [Effective cloud-native Java app development with Open Liberty in the Eclipse IDE](https://developer.ibm.com/articles/awb-effective-cloud-native-development-open-liberty-eclipse-ide)
  * Refactoring tools
    * Mono2Micro
      * [Mono2Micro documentation](https://www.ibm.com/docs/en/mono2micro?topic=mono2micro-overview) (docs)
      * [Using AI to refactor Java monoliths into microservices](https://www.youtube.com/watch?v=vN67fi1Yc0o) (video)
      * [Accelerate your journey to microservices with binary analysis](https://www.youtube.com/watch?v=86tsMDmoZBA) (video)
      * [Step-by-step instructions for Mono2Micro](https://heidloff.net/article/step-by-step-instructions-mono2micro/) (article)
      * [Licensing for Mono2Micro](https://www.ibm.com/docs/en/mono2micro?topic=overview-licensing) (docs)
      * [Links to trials](https://www.ibm.com/products/jsphere/tools) (ibm.com)


* Recommended order of steps and what to look out for ([issue](https://github.com/WASdev/websphere-and-liberty/issues/36))
  * eg migrate then update Java version, types of issues the migration report covers and what it doesn't, where to start when you receive the report)
* Matrix of Liberty features with levels of other IBM products ([issue](https://github.com/WASdev/websphere-and-liberty/issues/17))

# How to migrate to Liberty

## How to migrate operations to Liberty

* What to do when, suggested sequence of steps ([issue](https://github.com/WASdev/websphere-and-liberty/issues/36))

* Getting Liberty and deployment solutions (MoRE, EAR, Liberty on containers)
  * [Getting started with MoRE](https://wasdev.github.io/MoRE-Getting-Started/)
* [Demystifying Liberty for WebSphere administrators](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/) (article with embedded videos)
* Best practices for setting up operations for Liberty when coming from a tWAS operational environment ([issue](https://github.com/WASdev/websphere-and-liberty/issues/18))
* Liberty on VMs
  * KevinP's labs (internal; [issue](https://github.com/WASdev/websphere-and-liberty/issues/24))
* Liberty in containers
  * Best practices running Liberty in containers by Kevin Grigorenko
    * [Part 1](https://community.ibm.com/HigherLogic/System/DownloadDocumentFile.ashx?DocumentFileKey=7371c543-07b2-570d-337d-abb4242c3146) (video)
    * [Part 2](https://community.ibm.com/HigherLogic/System/DownloadDocumentFile.ashx?DocumentFileKey=0ff5d60b-1f7a-59db-8e8c-9549004e13b7) (video)
  * KevinP's labs (internal; [issue](https://github.com/WASdev/websphere-and-liberty/issues/24))
  * [cloud deployment guides](https://openliberty.io/guides/#cloud_deployment) (OL guides)
  * [Kubernetes guides](https://openliberty.io/guides/#kubernetes) (OL guides)
  * [Running WebSphere Liberty in a container](https://www.ibm.com/docs/en/was-liberty/base?topic=running-websphere-liberty-in-container) (WL docs)

| Topic | Resources available (description, link, and type)| Sources of info to create missing resources |
| --- | --- | --- |
| Operations: Moving from Admin Console to Liberty admin center, MoRE, etc. | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/37)) | [Demystifying Liberty for WebSphere administrators: Myth #3](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-3-liberty-doesn-t-have-an-admin-console6) (article with embedded videos); [Liberty Admin Center](https://openliberty.io/docs/latest/admin-center.html); [WebSphere admin console](https://www.ibm.com/docs/en/was/9.0.5?topic=clients-using-administrative-console); [wsadmin scripting](https://www.ibm.com/docs/en/was/9.0.5?topic=clients-getting-started-wsadmin-scripting);|
| Operations: How to secure the server configuration on Liberty | [Security Configuration Hardening docs](https://openliberty.io/docs/latest/security-hardening.html) (docs) |  | 
| Operations: How to do centralised management in Liberty | [Demystifying Liberty for WebSphere administrators: Myth #2](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-2-liberty-does-not-have-centralized-management4) (article with embedded videos) |
| Operations: How to load-balance across Liberty servers | [Demystifying Liberty for WebSphere administrators: Myth #5](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-5-it-is-very-hard-to-configure-liberty-with-ibm-http-server10) (article with embedded videos) |
| Operations: How to manage plugin config of dynamic routing in Liberty | [Demystifying Liberty for WebSphere administrators: Myth #5](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-5-it-is-very-hard-to-configure-liberty-with-ibm-http-server10) (article with embedded videos) |
| Operations: Licences and entitlement to run Liberty | [Demystifying Liberty for WebSphere administrators: Myth #8](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-8-i-don-t-have-licenses-to-run-liberty14) (article with embedded videos) |
| Operations: Messaging engine compatibility between tWAS and Liberty |  |
| Operations: How to script deployments on Liberty|  [Demystifying Liberty for WebSphere administrators: Myth #4](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-4-you-cannot-script-liberty8) (article with embedded videos)|
| Operations: How to do HTTP session persistence on Liberty | [Demystifying Liberty for WebSphere administrators: Myth #6](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-6-liberty-doesn-t-support-high-availability-ha-12) (article with embedded videos) |
| Operations: How to tune Liberty performance | [Threadpool tuning Liberty](https://openliberty.io/docs/latest/thread-pool-tuning.html); [Performance tuning Liberty](https://openliberty.io/docs/latest/performance-tuning.html); [Faster responses with HTTP response compression on Liberty](https://openliberty.io/blog/2020/04/22/http-response-compression.html); [Pre-populating database connections for better response times in the cloud](https://openliberty.io/blog/2020/09/09/pre-populating-db-connections.html); [Common performance tuning](https://publib.boulder.ibm.com/httpserv/cookbook/Recipes-WAS_Liberty_Recipes.html); [Some known migration issues mostly around performance](https://publib.boulder.ibm.com/httpserv/cookbook/Competition_and_Migration.html#Competition_and_Migration-WAS_Migration_Performance_Differences)(mostly tWAS to tWAS but some Java and Linux related points that would apply to going to Liberty on a newer Java); |
| Operations: Liberty on z/OS | Consider enabling SMF 120 records: HTTP requests may be monitored with [SMF 120 subtype 11 records](https://www.ibm.com/docs/en/was-liberty/nd?topic=erllz-smf-type-120-subtype-11-version-2-version-3-record-mapping). These records are enabled by adding the [zosRequestLogging-1.0](https://www.ibm.com/docs/en/was-liberty/nd?topic=zos-enabling-request-logging-liberty) feature to the server configuration and enabling SMF to capture those records. Java batch jobs may be monitored with [SMF 120 subtype 12 records](https://www.ibm.com/docs/en/was-liberty/nd?topic=zos-smf-type-120-subtype-12-record-mapping). These records are enabled by adding the [batchSMFLogging-1.0](https://www.ibm.com/docs/en/was-liberty/nd?topic=liberty-enabling-java-batch-smf-logging-zos) feature to the server configuration and enabling SMF to capture those records. Consider WLM classification: [zosWlm-1.0](https://www.ibm.com/docs/en/was-liberty/nd?topic=zos-enabling-workload-management-liberty)
Enable hardware cryptography | [Java 8](https://www.ibm.com/support/pages/node/6209109), [Java 11](https://www.ibm.com/support/pages/node/6840291), [Java 17](https://www.ibm.com/support/pages/node/6840291), or [Java 21](https://www.ibm.com/support/pages/node/6840291)| |
| Operations: How to run older programming models on Liberty | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/38)) |
| Operations: How to do high availability (HA) on Liberty | [Demystifying Liberty for WebSphere administrators: Myth #6](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-6-liberty-doesn-t-support-high-availability-ha-12) (article with embedded videos) |
| Operations: How to move to Liberty without going to the cloud | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/39)) |
| Operations: Can I use Liberty in exactly the same way as tWAS? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/40)) |
| Technical: Scaling, administration, clusters     | [Demystifying Liberty for WebSphere administrators](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/) (article with embedded videos) |
| How to optimize routing setup for HTTP routing (eg F5, NGINX, Apache mod_rewrite)? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/41)) |
| How to design continuous integration builds with Liberty's Maven plugin? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/42)) |
| Issues to look out for, differences between WebSphere and Liberty and how to handle them | (create post from Monica and Barbara's presentation, [issue](https://github.com/WASdev/websphere-and-liberty/issues/43)) |
| **Managing Deployment Scripts without WAS ND**    | [Demystifying Liberty for WebSphere administrators: Myth #4](https://developer.ibm.com/articles/demystifying-liberty-websphere-admins/#myth-4-you-cannot-script-liberty8) (article with embedded videos); Deployment best practices? ([issue](https://github.com/WASdev/websphere-and-liberty/issues/72)) | 
| Issues to look out for, differences between WebSphere and Liberty and how to handle them -  **Deploying Liberty on VM’s (Collectives or HTTP Proxy)**  | [Kevin's lab](https://techzone.ibm.com/collection/64073133d59dc60018783816) (internal) |
| Issues to look out for, differences between WebSphere and Liberty and how to handle them -  **How to configure Hardware Security Module (HSM) on z/OS on IBM Java on Liberty**    | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/44)) | 
| Hands-on demos/labs | [Tech Zone demos, VMs, presentations](https://techzone.ibm.com/collection/64073133d59dc60018783816); [Liberty to VMs](https://techzone.ibm.com/collection/64073133d59dc60018783816); [Liberty to OCP](https://techzone.ibm.com/collection/liberty-container-deployment-with-cp4apps-on-openshift-pot) (internal, [issue](https://github.com/WASdev/websphere-and-liberty/issues/24)) |
| How to migrate clusters, in particular session management and failover logic? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/45)) |
| How to update deployment pipelines for Liberty? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/46)) |


## How to migrate applications to run on Liberty

Tips: sequence and “how” for known cases
What to do when, suggested sequence of steps 

* Migrate and then update Java version 
* Issues to look out for, differences between WebSphere and Liberty and how to handle them 
* Transaction management
* Managing Deployment Scripts without WAS ND 
* Deploying Liberty on VM’s (Collectives or HTTP Proxy) 
* [Remote transaction propagation between Remote EJBs](https://community.ibm.com/community/user/blogs/laura-cowen1/2025/09/12/transaction-propagation-on-liberty)

| Topic | Resources available (description, link, and type)|
| --- | --- |
| Issues to look out for, differences between WebSphere and Liberty and how to handle them -  **Transaction management** |[add resources here] |
| Transaction propagation between remote EJBs   | [Transaction propagation on Liberty](https://community.ibm.com/community/user/blogs/laura-cowen1/2025/09/12/transaction-propagation-on-liberty) (article) | 
| How to do EJB lookups  | [Binding remote EJB names with Liberty](https://stackoverflow.com/questions/79555723/binding-remote-ejb-names-with-liberty) (forum); [Liberty Support for Custom JNDI Names for Enterprise Beans](https://openliberty.io/blog/2020/11/20/JNDI-gRPC-200012.html#jndi) (OL blog; also available on the [Red Hat Developer blog](https://developers.redhat.com/blog/2020/12/02/open-liberty-20-0-0-12-brings-support-for-grpc-custom-jndi-names-and-java-se-15#use_custom_jndi_names_to_look_up_or_inject_ejbs)) |
| How to migrate hardcoded `InitialContext` or `java:global` lookups? | See [InitialContext and java:global lookups](InitialContext-and-java%3Aglobal-lookups) ([issue](https://github.com/WASdev/websphere-and-liberty/issues/51)) |
| How to migrate SOAP endpoints using JAX-RPC? | [Automating JAX-RPC source code migration](https://community.ibm.com/community/user/viewdocument/20250109-cab-session-automating-j?CommunityKey=1348d157-c61b-417f-928a-179c3d0ffccb&tab=librarydocuments) (video) |
| How to migrate authentication using DatabaseServerLoginModule? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/48)) |
| How to validate migrated Filenet connections? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/49)) |
| How to migrate WebSphere SIBus JMS messaging? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/50)) |
| How to migrate hardcoded `InitialContext` or `java:global` lookups? | See [InitialContext and java:global lookups](InitialContext-and-java%3Aglobal-lookups) ([issue](https://github.com/WASdev/websphere-and-liberty/issues/51)) |
| How to migrate legacy Spring and Hibernate frameworks that don't support Java 17? Are there common pitfalls? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/52)) |
| What are the differences in classloader locations between tWAS and Liberty? | [Rules for migrating WebSphere traditional application class loading configuration to Liberty](https://www.ibm.com/support/pages/rules-migrating-websphere-traditional-application-class-loading-configuration-liberty) (IBM Support) (covers classloader hierarchies for tWAS and Liberty, migration rules for classloading, classloading libraries, classloading config); [Class loader configuration](https://openliberty.io/docs/latest/class-loader-library-config.html) (OL docs) |
| What are the differences in WAR structure between tWAS and Liberty? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/78)) |
| Does it matter if some apps use javax and others use jakarta? Is it necessary to migrate fully to Jakarta 10? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/54)) |
| How to validate integrations after migration? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/55)) |
| How to manage third-party dependencies (JARs) in Liberty? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/56)) |
| How to transition existing dashboards and alerts from WebSphere and other inputs to Liberty's JSON logging, MicroProfile Metrics, and OpenTelemetry? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/56)) |
| How to migrate certificates from WebSphere to Liberty's TLS setups for keyStore and SSL? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/58)) |
| How to transition WARs/EARs to Liberty? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/60)) |
| How to configure AD, LDAP, SPNEGO, SAML, OIDC on Liberty? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/61)) |
| Any compatibility issues to watch for moving from Java 8 (Oracle or IBM) to Java 17 (OpenJDK distributions)? | ([issue](https://github.com/WASdev/websphere-and-liberty/issues/62)) |
| How to automate JAX-RPC source code migration | [20250109 CAB session - Automating JAX-RPC source code migration](https://community.ibm.com/community/user/viewdocument/20250109-cab-session-automating-j?CommunityKey=1348d157-c61b-417f-928a-179c3d0ffccb&tab=librarydocuments) (video) |
| How to run Spring Boot apps on Liberty | [How to Containerize Your Spring Boot Application for Rapid Startup (DZone.com)](https://dzone.com/articles/containerize-spring-boot-app-for-rapid-startup); [Running a Spring Boot 3.x application WAR file on Liberty](https://openliberty.io/blog/2024/05/01/spring-boot-3.html); [all Spring Boot blog posts on openliberty.io](https://openliberty.io/blog/?search=spring); missing: "a complete demo/guide that connects our three flagship enterprise products (WebSphere, DB2, MQ) with a spring boot application using Liberty InstantOn to scale to zero on OpenShift and then also show how Semeru cloud compiler can be enabled with Liberty operators to reduce rampup time even more efficiently."; [Spring Boot performance](https://ibm-cloud.slack.com/archives/C30NGTBFS/p1753465423611499) (internal; [issue](https://github.com/WASdev/websphere-and-liberty/issues/63)) |
| Support for legacy versions of Spring and Struts | [Open Source Library Support announcement](https://www.ibm.com/docs/en/announcements/secure-java-applications-from-vulnerabilities-library-support-spring-library-support-struts) |

# Client case studies

(these should be organised/presented according to what they demo and/or by industry, etc so they're easily retrieved)

* [How to deploy an Open Liberty InstantOn app to OpenShift Local](https://thechalkboards.com/how-to-deploy-an-open-liberty-instanton-app-to-openshift-local/)
* [Modernizing Software Architecture with MicroProfile and Open Liberty](https://www.ibm.com/case-studies/blog/modernizing-software-architecture-with-microprofile-and-open-liberty)
* [Open Liberty in Action - Primeur’s data integration platform](https://openliberty.io/blog/2023/09/20/Primeur.html)
* [PowerM](https://www.ibm.com/case-studies/govt-dept-in-morocco)
* [Blue Cross Blue Shield of South Carolina](https://www.ibm.com/case-studies/bluecross-blueshield-of-south-carolina)
* [Redbridge](https://www.ibm.com/case-studies/redbridge)
* [FlowFactor](https://www.ibm.com/case-studies/flowfactor)
* [FlowFactor re InstantOn](https://www.ibm.com/new/announcements/ibm-websphere-liberty-announces-instanton-for-cloud-native-java)
* [Hera Spa](https://www.ibm.com/case-studies/hera-spa); [IDC report of dev efficiency with Liberty](https://www.ibm.com/account/reg/us-en/signup?formid=urx-52553); [Bernhardt](https://www.ibm.com/case-studies/bernhardt-furniture)
* [Alinma Bank](https://www.ibm.com/case-studies/alinma-bank-websphere-liberty)
* [Financial institution in Saudia Arabia](https://thechalkboards.com/websphere-liberty-and-the-value-of-websphere-hybrid-edition/)
* [Carey International](https://www.ibm.com/case-studies/carey-international)
* [Discover](https://www.ibm.com/think/insights/application-modernization-at-discover-the-need-to-modernize)
* [IBM CIO org](https://www.ibm.com/think/insights/ibm-cio-a-client-zero-to-application-modernization)
* [IBM CIO org 2](https://www.linkedin.com/pulse/modernizing-legacy-applications-kathryn-guarini/)
* [Canon Europe](https://www.ibm.com/case-studies/canoneuropevideo4)
* [GBM](https://www.ibm.com/case-studies/gbm)

# Training

* Training - developers
  * [Liberty Developer Essentials badge](https://www.credly.com/org/ibm/badge/liberty-developer-essentials) (free badge developers can earn through Credly)
  * [IBM Certified Developer – Cloud Native Java with IBM Liberty](https://www.ibm.com/training/certification/ibm-certified-developer-cloud-native-java-with-ibm-liberty-2023-C9004800) (certification exam)
* Training - operations
  * [Liberty: Installation and Multi-Server Management](https://www.ibm.com/training/course/liberty-installation-and-multi-server-management-ZA191G)


# Other resources
| Topic | Resources available (description, link, and type)|
| --- | --- |
| OSS libraries |[add resources here] |
| Documentation | [Liberty docs (apply to Open Liberty and WebSphere Liberty](https://openliberty.io/docs/latest/overview.html); [WebSphere Liberty docs (for features only available in WebSphere Liberty)](https://www.ibm.com/docs/en/was-liberty/base?topic=overview-where-find-liberty-documentation) |
| What's new in Liberty? | [Open Liberty release blog posts](https://openliberty.io/guides/); [Quarterly webinars](https://community.ibm.com/community/user/groups/community-home/recent-community-events?communitykey=5c4ba155-561a-4794-9883-bb0c6164e14e); [Open Liberty LinkedIn page](https://www.linkedin.com/company/openlibertyio) |
| Online forums | [WebSphere & Liberty TechXchange community](https://community.ibm.com/community/user/communities/community-home?CommunityKey=5c4ba155-561a-4794-9883-bb0c6164e14e); [WebSphere & Liberty Customer Advisory Board (CAB) TechXchange community](https://community.ibm.com/community/user/groups/community-home?CommunityKey=1348d157-c61b-417f-928a-179c3d0ffccb&tab=groupdetails) |
| Videos | [Laura's backups of ExpertTV etc](https://ibm.box.com/s/p5oiyeke5f46wqxwsw3y7ow157feb5i3) (internal); [Grace's video audit](https://ibm.box.com/s/fanhkrkddgz8fd8y0zaob9df4xv0k83a) (internal) Videos cover topics listed on this whole page but all videos probably need updating. |

# Suggested article/video ideas
* I can do x on tWAS, how do I do x on Liberty?
* Liberty operations for a tWAS operator
* Code changes probably not needed...but if they are...
 
# Source formats

Each link is labelled to indicate its format:

* _OL docs_: [Open Liberty docs](https://openliberty.io/docs)
* _OL guides_: [Open Liberty developer guides](https://openliberty.io/guides)
* _OL tools_: [Open Liberty starter](https://openliberty.io/start/) and [Liberty Tools for IDEs](https://openliberty.io/docs/latest/develop-liberty-tools.html)
* _OL blog_: [Open Liberty blog](https://openliberty.io/blog)
* _WL docs_: WebSphere Liberty docs
* _docs_: Other official product docs
* _IBM Support_: IBM Support article
* IBM Redbooks
  * _RB Liberty admin_: [IBM WebSphere Application Server V8.5 Administration and Configuration Guide for Liberty Profile](https://www.redbooks.ibm.com/redbooks/pdfs/sg248170.pdf)
* _IBM Developer_: article or tutorial on developer.ibm.com
* _slides_: various presentation slides
* _video_: video on YouTube or IBM site
* _article_: article on non-IBM website
* _forum_: Q & A site, such as StackOverflow
* _internal_: currently IBM-internal only
* _wip_: work in progress

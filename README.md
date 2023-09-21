# swe-articles
Articles and documentations about software engineering workflow processes, techniques, "best practices", and so on. Inspired by Prof. Gail Kaiser's COMS W4156 Advanced Software Engineering course.

## 👥 Human Scalability
### Teamwork Fundamentals
* [Coping with Hitchhikers and Couch Potatoes on Teams](https://www2.isye.gatech.edu/~jvandeva/Classes/4106/CouchPotatoes.pdf)
* [Pair Programming](https://martinfowler.com/articles/on-pair-programming.html)
* [Code Reviews](https://www.eferro.net/2021/09/code-reviews-synchronous-and.html)
### Version Control
* [Basic Version Control](https://github.com/git-guides)
* [Merging Changes](https://git-scm.com/docs/git-merge)
* [Auto-Merge](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/automatically-merging-a-pull-request)
* [Manual Resolution](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts)
* [Branches](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches)
* [Pull Requests](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests)
* [Release Tags](https://git-scm.com/book/en/v2/Git-Basics-Tagging)

## 🛠️ Code Readability and Maintainability
### Coding Style
* [Google Style Guides](https://google.github.io/styleguide/)
* Style Checkers
  * [checkstyle](https://github.com/checkstyle/checkstyle)
  * [SonarLint](https://www.sonarsource.com/products/sonarlint/)
  * Style-checking automation: [git pre-commit hook](https://git-scm.com/book/en/v2/Customizing-Git-Git-Hooks)
### Code Documentation
* [Google Engineering Practices Documentation](https://google.github.io/eng-practices/)
* [Documentation Best Practices](https://google.github.io/styleguide/docguide/best_practices.html)
* [Unit Tests are the Best Documentation](https://capgemini.github.io/development/unit-tests-as-documentation/)
* [README.md files](https://google.github.io/styleguide/docguide/READMEs.html)
* Documentation checker: [Vale](https://github.com/errata-ai/vale)

## 🛎️ Understanding What a Service Is
### Software Architecture 
Components of software architecture that constitute **applications**.
* [What Are Frontend and Backend in App Development?](https://www.lizard.global/blog/what-are-frontend-and-backend-in-app-development)
* [Frontend vs Backend](https://www.geeksforgeeks.org/frontend-vs-backend/)
* [Client-Server Model](https://www.geeksforgeeks.org/client-server-model/)
* [Three-Layered Application Architecture](https://vfunction.com/blog/the-benefits-of-a-three-layered-application-architecture/)
* [Software Architectural Design](https://www.geeksforgeeks.org/software-engineering-architectural-design/)
### Software-as-a-Service
Software delivery model for end users to access **software applications** over the internet.
* [What is SaaS?](https://www.salesforce.com/in/saas/)
### Application Programming Interfaces (APIs)
* [What is an API?](https://www.redhat.com/en/topics/api/what-are-application-programming-interfaces)
* [Most Popular APIs in 2022](https://www.postman.com/explore/most-popular-apis-this-year)
* [n0shake/Public-APIs](https://github.com/n0shake/Public-APIs)
* [public-apis/public-apis](https://github.com/public-apis/public-apis)
### Common Entry Points of APIs
* [Asynchronous Messages](https://www.mendix.com/blog/asynchronous-vs-synchronous-programming/)
* [Callbacks](https://medium.com/@cortneythomas/what-is-a-callback-8734a08605cb)
* [References to Data](https://thenewstack.io/the-fundamentals-of-data-api-design/)
### Additional Infrastructure Needed to Call Service Functions
* Remote procedure
  * [gRPC](https://grpc.io/)
* Message broker
  * [Apache Kafka]()
  * [RabbitMQ](https://aws.amazon.com/compare/the-difference-between-rabbitmq-and-kafka/)
* [REpresentational State Transfer(REST)](https://aws.amazon.com/what-is/restful-api/)
  * [Spring](https://spring.io/guides/tutorials/rest/)
### Non-Service Software Units with APIs
* [Frameworks](https://www.red-gate.com/simple-talk/development/other-development/the-difference-between-libraries-and-frameworks/)
### Microservices
* [4 Microservices Examples: Amazon, Netflix, Uber, and Etsy](https://blog.dreamfactory.com/microservices-examples/)

## 🔌 Technical Aspects of APIs
Previously, we have had a high-level view of what APIs are and examined their differences with applications. We now take a closer look at their technical details.

### RESTful APIs: the fundamentals
* [What is REST](https://restfulapi.net/)
* [API requests: GET vs. POST](https://www.diffen.com/difference/GET-vs-POST-HTTP-Requests)

### RESTful APIs: states
* [Stateful vs. Stateless: Understanding the Key Differences ](https://www.spiceworks.com/tech/cloud/articles/stateful-vs-stateless/)
* [Stateful vs Stateless Architecture](https://www.youtube.com/watch?v=P8D6P-6KVNM)
* [Stateful vs Stateless: Full Difference](https://www.interviewbit.com/blog/stateful-vs-stateless/)
* [Planning persistent storage](https://www.ibm.com/docs/en/cloud-private/3.2.x?topic=storage-planning-persistent)

### RESTful APIs: Java implementation
Kudos to Griffin Newbold for the following 2 articles.
* [Easily build a REST API with Spring Framework](https://medium.com/analytics-vidhya/easily-build-your-rest-api-with-spring-framework-80941c359d44)
* [Building REST services with Spring](https://spring.io/guides/tutorials/rest/)

### RPC-based APIs
* [RPC in Operating System](https://www.geeksforgeeks.org/remote-procedure-call-rpc-in-operating-system/)
* [What's the Difference Between RPC and REST?](https://aws.amazon.com/compare/the-difference-between-rpc-and-rest/)

### More API Architectures
* [Comparing API Architectural Styles: SOAP vs REST vs GraphQL vs RPC](https://www.altexsoft.com/blog/soap-vs-rest-vs-graphql-vs-rpc/)

### Stateful Architecture
REST APIs are stateless because, rather than relying on the server remembering previous requests, REST applications require each request to contain all of the information necessary for the server to understand it; since we have already investigated REST APIs, here are some examples of stateful architecture.
* [Stateful and stateless architecture design](https://www.linkedin.com/pulse/stateful-stateless-architecture-design-milad-rezaeighale/)
* [How Do Stateful Applications Work?](https://blog.dreamfactory.com/stateful-vs-stateless-web-app-design/#1)
* [Why Stateless Won](https://www.virtasant.com/blog/stateful-vs-stateless-architecture-why-stateless-won)

## 🌱 Real-World Case Studies

### C++ in Finance Industry
* [Trading Systems - CppCast](https://open.spotify.com/episode/0m7QrAe4Pn4As7A2eENs8n)

### Functional Programming Use Cases 
* [Fighting spam with Haskell](https://engineering.fb.com/2015/06/26/security/fighting-spam-with-haskell/)
* [Functional Programming at Verizon OnCue](http://cufp.org/2014/timothy-perrett-functional-programming-at-verizon-oncue.html)

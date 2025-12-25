---
kindle-sync:
  bookId: '36350'
  title: 'Fundamentals of Software Architecture: An Engineering Approach'
  author: Mark Richards and Neal Ford
  asin: B0849MPK73
  lastAnnotatedDate: '2023-10-28'
  bookImageUrl: 'https://m.media-amazon.com/images/I/9193iMIxVTL._SY160.jpg'
  highlightsCount: 46
---
# Fundamentals of Software Architecture
## Metadata
* Author: [Mark Richards and Neal Ford](https://www.amazon.comundefined)
* ASIN: B0849MPK73
* Reference: https://www.amazon.com/dp/B0849MPK73
* [Kindle link](kindle://book?action=open&asin=B0849MPK73)

## Highlights
The structure of the system, as illustrated in Figure 1-3, refers to the type of architecture style (or styles) the system is implemented in (such as microservices, layered, or microkernel). — location: [175](kindle://book?action=open&asin=B0849MPK73&location=175) ^ref-61583

---
The next factor that defines software architecture is architecture decisions. Architecture decisions define the rules for how a system should be constructed. — location: [188](kindle://book?action=open&asin=B0849MPK73&location=188) ^ref-53389

---
For example, an architect might make an architecture decision that only the business and services layers within a layered architecture can access the database — location: [190](kindle://book?action=open&asin=B0849MPK73&location=190) ^ref-277

---
The last factor in the definition of architecture is design principles. A design principle differs from an architecture decision in that a design principle is a guideline rather than a hard-and-fast rule. — location: [199](kindle://book?action=open&asin=B0849MPK73&location=199) ^ref-43835

---
There are eight core expectations placed on a software architect, irrespective of any given role, title, or job description: — location: [212](kindle://book?action=open&asin=B0849MPK73&location=212) ^ref-40692

---
Make architecture decisions Continually analyze the architecture Keep current with latest trends Ensure compliance with decisions Diverse exposure and experience Have business domain knowledge Possess interpersonal skills Understand and navigate politics — location: [213](kindle://book?action=open&asin=B0849MPK73&location=213) ^ref-43634

---
An architect is expected to define the architecture decisions and design principles used to guide technology decisions within the team, the department, or across the enterprise. — location: [218](kindle://book?action=open&asin=B0849MPK73&location=218) ^ref-60754

---
An architect is expected to continually analyze the architecture and current technology environment and then recommend solutions for improvement. — location: [230](kindle://book?action=open&asin=B0849MPK73&location=230) ^ref-45014

---
An architect is expected to keep current with the latest technology and industry trends. — location: [241](kindle://book?action=open&asin=B0849MPK73&location=241) ^ref-50745

---
An architect is expected to ensure compliance with architecture decisions and design principles. — location: [247](kindle://book?action=open&asin=B0849MPK73&location=247) ^ref-62332

---
An effective software architect should be aggressive in seeking out opportunities to gain experience in multiple languages, platforms, and technologies. — location: [263](kindle://book?action=open&asin=B0849MPK73&location=263) ^ref-27060

---
Everything in software architecture is a trade-off. — location: [457](kindle://book?action=open&asin=B0849MPK73&location=457) ^ref-54592

---
Why is more important than how. — location: [464](kindle://book?action=open&asin=B0849MPK73&location=464) ^ref-38039

---
We use modularity to describe a logical grouping of related code, — location: [704](kindle://book?action=open&asin=B0849MPK73&location=704) ^ref-1299

---
Cohesion — location: [756](kindle://book?action=open&asin=B0849MPK73&location=756) ^ref-60251

---
Cohesion refers to what extent the parts of a module should be contained within the same module. — location: [757](kindle://book?action=open&asin=B0849MPK73&location=757) ^ref-26769

---
In other words, it is a measure of how related the parts are to one another. — location: [757](kindle://book?action=open&asin=B0849MPK73&location=757) ^ref-54854

---
Ideally, a cohesive module is one where all the parts should be packaged together, — location: [758](kindle://book?action=open&asin=B0849MPK73&location=758) ^ref-24315

---
Computer scientists have defined a range of cohesion measures, listed here from best to worst: — location: [761](kindle://book?action=open&asin=B0849MPK73&location=761) ^ref-15393

---
Functional cohesion Every part of the module is related to the other, and the module contains everything essential to function. — location: [762](kindle://book?action=open&asin=B0849MPK73&location=762) ^ref-56740

---
Sequential cohesion Two modules interact, where one outputs data that becomes the input for the other. — location: [763](kindle://book?action=open&asin=B0849MPK73&location=763) ^ref-46437

---
Communicational cohesion Two modules form a communication chain, where each operates on information and/or contributes to some output. — location: [765](kindle://book?action=open&asin=B0849MPK73&location=765) ^ref-9463

---
Procedural cohesion Two modules must execute code in a particular order. — location: [767](kindle://book?action=open&asin=B0849MPK73&location=767) ^ref-35655

---
Temporal cohesion Modules are related based on timing dependencies. — location: [769](kindle://book?action=open&asin=B0849MPK73&location=769) ^ref-35168

---
Logical cohesion The data within modules is related logically but not functionally. — location: [772](kindle://book?action=open&asin=B0849MPK73&location=772) ^ref-10616

---
Coincidental cohesion Elements in a module are not related other than being in the same source file; this represents the most negative form of cohesion. — location: [776](kindle://book?action=open&asin=B0849MPK73&location=776) ^ref-1383

---
Are those the only two operations for Order Maintenance? If so, it may make sense to collapse those operations back into Customer Maintenance. — location: [787](kindle://book?action=open&asin=B0849MPK73&location=787) ^ref-34781

---
Does Order Maintenance require so much knowledge of Customer information that separating the two modules would require a high degree of coupling to make it functional? — location: [789](kindle://book?action=open&asin=B0849MPK73&location=789) ^ref-34799

---
P increases by one for any method that doesn’t access a particular shared field and Q decreases by one for methods that do share a particular shared field. — location: [801](kindle://book?action=open&asin=B0849MPK73&location=801) ^ref-47413

---
LCOM The sum of sets of methods not shared via sharing fields — location: [808](kindle://book?action=open&asin=B0849MPK73&location=808) ^ref-45951

---
Consider a class with private fields a and b. Many of the methods only access a, and many other methods only access b. The sum of the sets of methods not shared via sharing fields (a and b) is high; therefore, this class reports a high LCOM score, indicating that it scores high in lack of cohesion in methods. — location: [809](kindle://book?action=open&asin=B0849MPK73&location=809) ^ref-40157

---
In Class X, the LCOM score is low, indicating good structural cohesion. — location: [815](kindle://book?action=open&asin=B0849MPK73&location=815) ^ref-4879

---
Class Z shows mixed cohesion, where developers could refactor the last field/method combination into its own class. — location: [817](kindle://book?action=open&asin=B0849MPK73&location=817) ^ref-51753

---
Afferent coupling measures the number of incoming connections to a code artifact (component, class, function, and so on). Efferent coupling measures the outgoing connections to other code artifacts. — location: [827](kindle://book?action=open&asin=B0849MPK73&location=827) ^ref-59573

---
while a purely functional view of component design might yield a single component to handle user interaction, analyzing the architecture characteristics will lead to a subdivision. — location: [2116](kindle://book?action=open&asin=B0849MPK73&location=2116) ^ref-21259

---
create an initial component design based on general knowledge of the system and how they choose to decompose it, based on technical or domain partitioning. — location: [2136](kindle://book?action=open&asin=B0849MPK73&location=2136) ^ref-58997

---
In Figure 8-9, the architect has basically taken each entity identified in the requirements and made a Manager component based on that entity. This isn’t an architecture; it’s an object-relational mapping (ORM) of a framework to a database. — location: [2144](kindle://book?action=open&asin=B0849MPK73&location=2144) ^ref-50600

---
If an architect’s needs require merely a simple mapping from a database to a user interface, full-blown architecture isn’t necessary; one of these frameworks will suffice. — location: [2160](kindle://book?action=open&asin=B0849MPK73&location=2160) ^ref-54210

---
The entity trap anti-pattern arises when an architect incorrectly identifies the database relationships as workflows in the application, a correspondence that rarely manifests in the real world. — location: [2161](kindle://book?action=open&asin=B0849MPK73&location=2161) ^ref-29298

---
The actor/actions approach is a popular way that architects use to map requirements to components. — location: [2167](kindle://book?action=open&asin=B0849MPK73&location=2167) ^ref-29186

---
architects identify actors who perform activities with the application and the actions those actors may perform. — location: [2168](kindle://book?action=open&asin=B0849MPK73&location=2168) ^ref-61871

---
In event storming, the architect assumes the project will use messages and/or events to communicate between the various components. — location: [2176](kindle://book?action=open&asin=B0849MPK73&location=2176) ^ref-65423

---
To that end, the team tries to determine which events occur in the system based on requirements and identified roles, and build components around those event and message handlers. — location: [2177](kindle://book?action=open&asin=B0849MPK73&location=2177) ^ref-14192

---
The workflow approach models the components around workflows, much like event storming, but without the explicit constraints of building a message-based system. — location: [2182](kindle://book?action=open&asin=B0849MPK73&location=2182) ^ref-39369

---
A workflow approach identifies the key roles, determines the kinds of workflows these roles engage in, and builds components around the identified activities. — location: [2183](kindle://book?action=open&asin=B0849MPK73&location=2183) ^ref-53335

---
If a team has no special constraints and is looking for a good general-purpose component decomposition, the Actor/Actions approach works well as a generic solution. — location: [2190](kindle://book?action=open&asin=B0849MPK73&location=2190) ^ref-44317

---

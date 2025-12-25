---
kindle-sync:
  bookId: '22598'
  title: >-
    Event-Driven Architecture in Golang: Building complex systems with
    asynchronicity and eventual consistency
  author: Michael Stack
  asin: B0B2DPFJN4
  lastAnnotatedDate: '2024-09-27'
  bookImageUrl: 'https://m.media-amazon.com/images/I/81tAOKPn4NL._SY160.jpg'
  highlightsCount: 125
---
# Event-Driven Architecture in Golang
## Metadata
* Author: [Michael Stack](https://www.amazon.comundefined)
* ASIN: B0B2DPFJN4
* Reference: https://www.amazon.com/dp/B0B2DPFJN4
* [Kindle link](kindle://book?action=open&asin=B0B2DPFJN4)

## Highlights
Event-driven architecture (EDA) is the foundational design of an application’s communication of state changes around an asynchronous exchange of messages called events. — location: [508](kindle://book?action=open&asin=B0B2DPFJN4&location=508) ^ref-51415

---
Three different uses or patterns exist that can be called EDA individually or altogether, as follows: Event notifications Event-carried state transfer Event sourcing — location: [534](kindle://book?action=open&asin=B0B2DPFJN4&location=534) ^ref-59770

---
A notification event typically carries the absolute minimum state, perhaps even just the identifier (ID) of an entity or the exact time of the occurrence of their payload. — location: [541](kindle://book?action=open&asin=B0B2DPFJN4&location=541) ^ref-65070

---
event-carried state transfer is a push model where data changes are sent out to be consumed by any components that might be interested. — location: [558](kindle://book?action=open&asin=B0B2DPFJN4&location=558) ^ref-3565

It doesn't include just an idea but all the information.

---
more detail could be added to provide as much detail as possible, — location: [565](kindle://book?action=open&asin=B0B2DPFJN4&location=565) ^ref-49310

---
Instead of capturing changes as irreversible modifications to a single record, those changes are stored as events. These changes or streams of events can be read and processed to recreate the final state of an entity when it is needed again. — location: [574](kindle://book?action=open&asin=B0B2DPFJN4&location=574) ^ref-48248

---
the event. In EDA terms, it is an occurrence that has happened in the application. — location: [589](kindle://book?action=open&asin=B0B2DPFJN4&location=589) ^ref-54915

---
The event itself is in the past and it is an immutable fact. — location: [590](kindle://book?action=open&asin=B0B2DPFJN4&location=590) ^ref-10098

---
Events should carry enough data to be useful in capturing the change in the application state that they’re meant to communicate. — location: [598](kindle://book?action=open&asin=B0B2DPFJN4&location=598) ^ref-62052

---
The defining characteristic of a message queue is its lack of event retention. All events put into a message queue have a limited lifetime. — location: [609](kindle://book?action=open&asin=B0B2DPFJN4&location=609) ^ref-34075

---
When you add event retention to a message queue, you get an event stream. — location: [618](kindle://book?action=open&asin=B0B2DPFJN4&location=618) ^ref-8878

---
Unlike message queues, which will eventually return to their default empty state, an event stream will continue to grow indefinitely until events are removed by outside forces, such as being configured with a maximum stream length or archived based on their age. — location: [621](kindle://book?action=open&asin=B0B2DPFJN4&location=621) ^ref-29132

---
When you need retention and the ability to replay events, an event stream should be used instead of a message queue. — location: [626](kindle://book?action=open&asin=B0B2DPFJN4&location=626) ^ref-1946

---
As the name implies, an event store is an append-only repository for events. — location: [628](kindle://book?action=open&asin=B0B2DPFJN4&location=628) ^ref-54795

---
Event stores are used in conjunction with event sourcing to track changes to entities. — location: [635](kindle://book?action=open&asin=B0B2DPFJN4&location=635) ^ref-31867

---
When some state in the application has changed, the producer will publish an event representing the change into the appropriate queue. — location: [638](kindle://book?action=open&asin=B0B2DPFJN4&location=638) ^ref-46094

---
The producers of the events will publish it without knowing what the consumers might be listening to. It is essentially a fire-and-forget operation. — location: [640](kindle://book?action=open&asin=B0B2DPFJN4&location=640) ^ref-18281

---
Consumers subscribe to and read events from queues. — location: [642](kindle://book?action=open&asin=B0B2DPFJN4&location=642) ^ref-15189

---
An event-driven application can be more agile in its development. Less coordination between teams is required when introducing new components to an application. — location: [714](kindle://book?action=open&asin=B0B2DPFJN4&location=714) ^ref-17465

---
aside. A small team can stand up a new component without disrupting the work of other teams or the flow of existing processes. — location: [717](kindle://book?action=open&asin=B0B2DPFJN4&location=717) ^ref-23683

---
Components that communicate using events make it easier for new components and processes to come online — location: [727](kindle://book?action=open&asin=B0B2DPFJN4&location=727) ^ref-64047

---
Eventual consistency is a challenge for any distributed application. Changes in the application state may not be immediately available. — location: [750](kindle://book?action=open&asin=B0B2DPFJN4&location=750) ^ref-30404

---
dual write refers to any time you’re changing the application state in two or more places during an operation. — location: [755](kindle://book?action=open&asin=B0B2DPFJN4&location=755) ^ref-2964

---
If the events we intend to publish never make it to the event broker, then our state changes cannot be shared, and post-operation operations will never happen. — location: [757](kindle://book?action=open&asin=B0B2DPFJN4&location=757) ^ref-43154

---
Each component may not have the final state of the application when queried, but it will eventually. — location: [769](kindle://book?action=open&asin=B0B2DPFJN4&location=769) ^ref-29950

---
Choreography: The components each individually know about the work they must do, and which step comes next — location: [781](kindle://book?action=open&asin=B0B2DPFJN4&location=781) ^ref-54730

---
Orchestration: The components know very little about their role and are called on to do their part by a centralized orchestrator — location: [783](kindle://book?action=open&asin=B0B2DPFJN4&location=783) ^ref-32025

---
One of the disadvantages of EDA is being able to publish an event and not necessarily knowing if anything is consuming that — location: [792](kindle://book?action=open&asin=B0B2DPFJN4&location=792) ^ref-18806

---
The Ubiquitous Language (UL) principle requires every domain-specific term to have a single meaning within a bounded context. — location: [870](kindle://book?action=open&asin=B0B2DPFJN4&location=870) ^ref-39348

---
To hammer the point home, use the UL everywhere in code. It should drive the names of your function names, the structs, the variables, and the processes that you develop. — location: [877](kindle://book?action=open&asin=B0B2DPFJN4&location=877) ^ref-55318

---
When the UL is being spoken but confusion starts to appear, it could be a sign that the domain model is undergoing an evolution, — location: [880](kindle://book?action=open&asin=B0B2DPFJN4&location=880) ^ref-43985

---
Core domains: Critical components of the application that are unique or provide a competitive advantage to the business. — location: [885](kindle://book?action=open&asin=B0B2DPFJN4&location=885) ^ref-47651

---
Supporting domains: The utility components that provide functionality that supports the core business. — location: [887](kindle://book?action=open&asin=B0B2DPFJN4&location=887) ^ref-18362

---
Generic domains: Components that are unrelated to the core business but necessary for it to function. — location: [890](kindle://book?action=open&asin=B0B2DPFJN4&location=890) ^ref-48614

---
It wouldn’t make sense to devote teams to develop this functionality when so many solutions exist. — location: [891](kindle://book?action=open&asin=B0B2DPFJN4&location=891) ^ref-5586

---
What goes into the model should be limited to the data and behaviors that are relevant to the problem domain, not everything possible in an attempt at modeling reality. — location: [907](kindle://book?action=open&asin=B0B2DPFJN4&location=907) ^ref-46857

---
The point of a domain model is to solve problems identified in the domain. — location: [908](kindle://book?action=open&asin=B0B2DPFJN4&location=908) ^ref-12292

---
Every model belongs to a bounded context, which is a component of the application. — location: [917](kindle://book?action=open&asin=B0B2DPFJN4&location=917) ^ref-41525

---
The purpose of context mapping is to recognize the relationships the models will have with other models and to also show the relationship between teams. — location: [942](kindle://book?action=open&asin=B0B2DPFJN4&location=942) ^ref-64039

---
concerns. The purpose of the architecture is to keep the domain free of any outside influences such as database specifics or framework concerns. — location: [974](kindle://book?action=open&asin=B0B2DPFJN4&location=974) ^ref-16024

---
Each outside dependency the application used would be broken — location: [998](kindle://book?action=open&asin=B0B2DPFJN4&location=998) ^ref-53692

---
up into two parts – a port or interface, and an adapter or implementation. — location: [999](kindle://book?action=open&asin=B0B2DPFJN4&location=999) ^ref-33680

---
He declared that “source code dependencies can only point inwards” as the most important aspect of domain-centric architectures. — location: [1029](kindle://book?action=open&asin=B0B2DPFJN4&location=1029) ^ref-46183

---
This layer of the application has no other dependencies and is free of any references to external concerns or application services. — location: [1063](kindle://book?action=open&asin=B0B2DPFJN4&location=1063) ^ref-33001

---
The application layer will also define the interfaces that external concerns will be using to interact with the application. — location: [1067](kindle://book?action=open&asin=B0B2DPFJN4&location=1067) ^ref-43431

---
The application layer may only ever depend on the domain layer and cannot reference external concerns. — location: [1068](kindle://book?action=open&asin=B0B2DPFJN4&location=1068) ^ref-31015

---
Communication between the adapters and the application happens only through the ports and the Data Transfer Objects (DTOs) that they have created to represent the requests and responses. — location: [1080](kindle://book?action=open&asin=B0B2DPFJN4&location=1080) ^ref-14295

---
A domain-centric architecture application will be highly testable and be cheaper to maintain in the long run. — location: [1094](kindle://book?action=open&asin=B0B2DPFJN4&location=1094) ^ref-39510

---
Command and Query Responsibility Segregation (CQRS) is a simple pattern to define. Objects are split into two new objects, with one being responsible for commands and the other responsible for queries. — location: [1109](kindle://book?action=open&asin=B0B2DPFJN4&location=1109) ^ref-54760

---
Command: Performs a mutation of the application state — location: [1117](kindle://book?action=open&asin=B0B2DPFJN4&location=1117) ^ref-61976

---
Query: Returns application state to the caller — location: [1118](kindle://book?action=open&asin=B0B2DPFJN4&location=1118) ^ref-16032

---
With an application divided into a command side and a query side, you can apply different security models to each side or decide to reduce the complexity of your service objects. You may continue to use the same database but use an ORM on one side and raw SQL for performance purposes on the other. — location: [1136](kindle://book?action=open&asin=B0B2DPFJN4&location=1136) ^ref-42009

---
Moving your queries over to a new data store such as a NoSQL, key-value, document, or graph database may be necessary to keep up with the load. — location: [1145](kindle://book?action=open&asin=B0B2DPFJN4&location=1145) ^ref-27815

---
Applying CQRS to the entire service gets you two services that can be scaled separately; they can be maintained by different teams and have entirely different technology stacks. — location: [1151](kindle://book?action=open&asin=B0B2DPFJN4&location=1151) ^ref-60954

---
When to consider CQRS — location: [1153](kindle://book?action=open&asin=B0B2DPFJN4&location=1153) ^ref-40717

---
Your system experiences a much larger amount of read operations than write operations. — location: [1155](kindle://book?action=open&asin=B0B2DPFJN4&location=1155) ^ref-21963

---
Security is applied differently for writes and reads; — location: [1158](kindle://book?action=open&asin=B0B2DPFJN4&location=1158) ^ref-45093

---
You are using event-driven patterns such as event sourcing. — location: [1159](kindle://book?action=open&asin=B0B2DPFJN4&location=1159) ^ref-53850

---
You have complex read patterns that bloat or complicate the model. — location: [1160](kindle://book?action=open&asin=B0B2DPFJN4&location=1160) ^ref-52899

---
You want the data to be available when writing is not possible. — location: [1162](kindle://book?action=open&asin=B0B2DPFJN4&location=1162) ^ref-59430

---
CQRS is not, in my opinion, an event-driven pattern. It can be used entirely without any kind of events or asynchronous approaches. — location: [1166](kindle://book?action=open&asin=B0B2DPFJN4&location=1166) ^ref-31577

---
The intended behavior of a user’s action is frequently lost behind the usage of basic commands such as UpdateUser in this type of UI. — location: [1175](kindle://book?action=open&asin=B0B2DPFJN4&location=1175) ^ref-13984

---
Monolithic architecture This is an application that is typically built from a single code base and is deployed as a single resource. — location: [1186](kindle://book?action=open&asin=B0B2DPFJN4&location=1186) ^ref-51464

---
The architecture also gets an unfair amount of negativity regarding the messy code that goes into the development of a monolith. That negativity is unfair because that can happen with any code base and has to do with bad design. — location: [1195](kindle://book?action=open&asin=B0B2DPFJN4&location=1195) ^ref-3036

---
If we apply DDD and a domain-centric architecture to our existing monolithic application, we can refactor it toward a modular monolith architecture. — location: [1200](kindle://book?action=open&asin=B0B2DPFJN4&location=1200) ^ref-41556

---
The advantages of microservices over a monolithic application are that they’re independently deployable and can be independently scaled. — location: [1211](kindle://book?action=open&asin=B0B2DPFJN4&location=1211) ^ref-58416

---
A modular monolith is the recommended architecture to start with for any project of reasonable complexity. — location: [1218](kindle://book?action=open&asin=B0B2DPFJN4&location=1218) ^ref-39210

---
After the application has outgrown the module monolith architecture, the team will be able to very easily extract the modules into microservices when needed to begin taking advantage of the benefits of the microservices architecture. — location: [1220](kindle://book?action=open&asin=B0B2DPFJN4&location=1220) ^ref-30090

---
EventStorming is a fun and engaging workshop that uses colorful sticky notes to quickly visualize the building blocks of the flows that make up your application. — location: [1278](kindle://book?action=open&asin=B0B2DPFJN4&location=1278) ^ref-16594

---
A domain event (orange) represents something that has an impact on your system and may occur either inside or outside. It should be written in the past tense. — location: [1285](kindle://book?action=open&asin=B0B2DPFJN4&location=1285) ^ref-29186

---
A command (blue) is an action or decision that is invoked by users or policies. — location: [1287](kindle://book?action=open&asin=B0B2DPFJN4&location=1287) ^ref-50270

---
A policy (lilac) is a business rule that can be identified by listening for the phrase “whenever <x>, then <y>.” — location: [1289](kindle://book?action=open&asin=B0B2DPFJN4&location=1289) ^ref-64499

---
An aggregate (tan) is a group of domain entities acted on as a single unit. — location: [1291](kindle://book?action=open&asin=B0B2DPFJN4&location=1291) ^ref-23171

---
An external system (pink) is a third-party system that is external to an application. — location: [1292](kindle://book?action=open&asin=B0B2DPFJN4&location=1292) ^ref-27991

---
Data (green) is information recorded in the system or is the required information for commands and business rules. — location: [1294](kindle://book?action=open&asin=B0B2DPFJN4&location=1294) ^ref-40547

---
An actor (yellow) is a user, role, or persona that creates actions in our system. — location: [1296](kindle://book?action=open&asin=B0B2DPFJN4&location=1296) ^ref-32794

---
A UI (white) is an interface example or screen mockup. — location: [1299](kindle://book?action=open&asin=B0B2DPFJN4&location=1299) ^ref-44874

---
The modules will not create any connections to the infrastructure themselves: — location: [1844](kindle://book?action=open&asin=B0B2DPFJN4&location=1844) ^ref-34718

---
The interface definition is kept close to the consumer, ideally in the same package or file. It is also defined to be as small as possible, only requiring the methods that the consumer would need to use. — location: [1880](kindle://book?action=open&asin=B0B2DPFJN4&location=1880) ^ref-21218

---
On the other hand, when working with ports and adapters, we want to define contracts for the interactions with our applications. This often means we will be defining larger interfaces that work as the contracts for the application adapter implementations. — location: [1884](kindle://book?action=open&asin=B0B2DPFJN4&location=1884) ^ref-41533

---
A composition root is the part of an application where you bring the infrastructure, configuration, and application components together: — location: [1907](kindle://book?action=open&asin=B0B2DPFJN4&location=1907) ^ref-53149

---
The composition root is also where dependency injection takes place, and an application object graph will be constructed. — location: [1911](kindle://book?action=open&asin=B0B2DPFJN4&location=1911) ^ref-60497

---
The communication between the modules is entirely synchronous and uses protocol buffers and gRPC. — location: [1936](kindle://book?action=open&asin=B0B2DPFJN4&location=1936) ^ref-37394

---
there are two reasons that bounded contexts will need to integrate: They need data that exists in another bounded context They need another bounded context to perform an action — location: [2000](kindle://book?action=open&asin=B0B2DPFJN4&location=2000) ^ref-13035

---
When a bounded context needs data belonging to another bounded context, it has three options: — location: [2004](kindle://book?action=open&asin=B0B2DPFJN4&location=2004) ^ref-11414

---
Share the database where the data is stored — location: [2005](kindle://book?action=open&asin=B0B2DPFJN4&location=2005) ^ref-65243

---
Push the data from the owner to all interested components Pull the data from the owner when it is needed — location: [2006](kindle://book?action=open&asin=B0B2DPFJN4&location=2006) ^ref-36450

---
When you push data out, you will be sending it to a list of known interested components. This is a maintenance nightmare. — location: [2010](kindle://book?action=open&asin=B0B2DPFJN4&location=2010) ^ref-53100

---
To get a command to the bounded context that needs it, two options come to mind: Push the command to the commanded component Poll for new commands from the commanding component — location: [2036](kindle://book?action=open&asin=B0B2DPFJN4&location=2036) ^ref-13572

---
In an event-driven application and even in an application that is not event-driven, you will encounter several different kinds of events: Domain events – synchronous events that come from domain-driven design Event sourcing events – serialized events that record state changes for an aggregate Integration events – events that exchange state with other components of an application — location: [2070](kindle://book?action=open&asin=B0B2DPFJN4&location=2070) ^ref-55538

---
A domain event is a concept that comes from domain-driven design. It is used to inform other parts of a bounded context about state changes. The events can be handled asynchronously but will most often be handled synchronously within the same process that spawned them. — location: [2076](kindle://book?action=open&asin=B0B2DPFJN4&location=2076) ^ref-27564

---
An event sourcing event is one that shares a lot in common with a domain event. These events will need to be serialized into a format so that they can be stored in event streams. Whereas domain events are only accessible during the duration of the current process, these events are retained for as long as they are needed. Event sourcing events also belong to an aggregate and will be accompanied by metadata containing the identity of the aggregate and when the event occurred. — location: [2081](kindle://book?action=open&asin=B0B2DPFJN4&location=2081) ^ref-58974

---
An integration event is one that is used to communicate state changes across context boundaries. Like the event sourcing event, it too is serialized into a format that allows it to be shared with other modules and applications. — location: [2088](kindle://book?action=open&asin=B0B2DPFJN4&location=2088) ^ref-38748

---
end. Integration events are strictly asynchronous and use an event broker to decouple the event producer from the event consumers. — location: [2091](kindle://book?action=open&asin=B0B2DPFJN4&location=2091) ^ref-4390

---
a domain event is a domain-driven design pattern that encapsulates a change in the system that is important to the domain experts. — location: [2097](kindle://book?action=open&asin=B0B2DPFJN4&location=2097) ^ref-18986

---
When important events happen in our system, they are often accompanied by rules or side effects. We may have a rule that when the OrderCreated event happens in our system, we send a notification to the customer. — location: [2098](kindle://book?action=open&asin=B0B2DPFJN4&location=2098) ^ref-54977

---
Domain events will not be shared outside of the bounded context, module, or microservice they belong to. — location: [2170](kindle://book?action=open&asin=B0B2DPFJN4&location=2170) ^ref-1151

---
We can put whatever we want into them so long as we are still treating them as immutable carriers of state We will not need to be concerned with anyone subscribing to them without knowing; therefore, there is no risk of making changes to them and breaking things unintentionally They live a very short amount of time and do not need to be serialized or versioned to be stored in any database or stream — location: [2171](kindle://book?action=open&asin=B0B2DPFJN4&location=2171) ^ref-18585

---
These domain events are transient and disappear once the process ends. — location: [2294](kindle://book?action=open&asin=B0B2DPFJN4&location=2294) ^ref-56377

---
Event sourcing is a pattern of recording each change to an aggregate into an append-only stream. To reconstruct an aggregate’s final state, we must read events sequentially and apply them to the aggregate. — location: [2314](kindle://book?action=open&asin=B0B2DPFJN4&location=2314) ^ref-31856

---
we have lost both the previous price and the intent of the change. — location: [2323](kindle://book?action=open&asin=B0B2DPFJN4&location=2323) ^ref-8200

---
Event sourcing implementations should use event stores that provide strong consistency guarantees and optimistic concurrency control. — location: [2327](kindle://book?action=open&asin=B0B2DPFJN4&location=2327) ^ref-56081

---
when two or more modifications are made concurrently, only the first modification can add events to the stream. — location: [2328](kindle://book?action=open&asin=B0B2DPFJN4&location=2328) ^ref-9316

---
Event streaming is when events are used to communicate state changes with other bounded contexts of an application. — location: [2333](kindle://book?action=open&asin=B0B2DPFJN4&location=2333) ^ref-11602

---
Event sourcing is when events are used to keep a history of the changes in a single context and can be considered an implementation detail and not an architectural choice that has application-wide ramifications. — location: [2334](kindle://book?action=open&asin=B0B2DPFJN4&location=2334) ^ref-36154

---
Event sourcing is implemented and contained within a single context boundary, whereas event streaming is typically used to integrate multiple context boundaries. — location: [2341](kindle://book?action=open&asin=B0B2DPFJN4&location=2341) ^ref-21120

---
an event streaming system is always going to be eventually consistent. An event-sourced system will have the same level of consistency as the database it is used with. — location: [2343](kindle://book?action=open&asin=B0B2DPFJN4&location=2343) ^ref-51234

---
You will not be able to search for your data with complex queries, and you will need to build other ways to access your data besides simple identity lookups. — location: [2347](kindle://book?action=open&asin=B0B2DPFJN4&location=2347) ^ref-38890

---
What we used before as events will now be used as event payloads. — location: [2384](kindle://book?action=open&asin=B0B2DPFJN4&location=2384) ^ref-29369

---
The event is a private struct that embeds Entity and contains only private fields. The use of EventOption will be the only way to modify these values outside of the ddd package. — location: [2416](kindle://book?action=open&asin=B0B2DPFJN4&location=2416) ^ref-5201

---
When you use notifications, you are expecting the interested consumers to eventually make a call back to you to retrieve more information, — location: [3267](kindle://book?action=open&asin=B0B2DPFJN4&location=3267) ^ref-61422

---
State transfer is great for interested consumers to build a local representation of the data so that it may handle future requests independently. — location: [3298](kindle://book?action=open&asin=B0B2DPFJN4&location=3298) ^ref-5285

---
Stateful events may contain only the data related to the specific change, or they can contain complete old and new representations of the resource, or a delta of a resource that was altered after the change was applied. — location: [3308](kindle://book?action=open&asin=B0B2DPFJN4&location=3308) ^ref-27984

---
Finally, events should never contain information that was received from another domain. For example, an event coming from a sales domain should not include a shipping schedule that it received from the warehouse domain. — location: [3310](kindle://book?action=open&asin=B0B2DPFJN4&location=3310) ^ref-60793

---
Eventual consistency is constant in distributed applications and especially in event-driven applications. — location: [3320](kindle://book?action=open&asin=B0B2DPFJN4&location=3320) ^ref-57766

---
is: An eventually consistent system that has stopped receiving modifications to an item will eventually return the same last update across the system. — location: [3323](kindle://book?action=open&asin=B0B2DPFJN4&location=3323) ^ref-19173

---
At the center of a 2PC is a coordinator that sends the Prepare and Commit messages to all the participants. During the Prepare phase, each participant may respond positively to signify they have started a local transaction and are ready to proceed. — location: [4398](kindle://book?action=open&asin=B0B2DPFJN4&location=4398) ^ref-52307

---
When it is implemented correctly and used in a preferably very well-tested system, it can offer very strong consistency as it has all ACID guarantees. — location: [4409](kindle://book?action=open&asin=B0B2DPFJN4&location=4409) ^ref-5024

---
A saga is a sequence of steps that define the actions and compensating actions for the system components that are involved, also known as the saga participants. — location: [4424](kindle://book?action=open&asin=B0B2DPFJN4&location=4424) ^ref-43080

---
The saga steps may use a local ACID transaction, but any changes that are made will be visible to concurrent operations while the other steps are being run. — location: [4428](kindle://book?action=open&asin=B0B2DPFJN4&location=4428) ^ref-51254

---
Since there are no resources tied up in a database blocking other work, we can build a saga that could have a lifetime of several seconds, minutes, or even longer: — location: [4430](kindle://book?action=open&asin=B0B2DPFJN4&location=4430) ^ref-37600

---
A saga may be a collaborative effort between participants and be choreographed, alternatively there can be a saga execution coordinator that orchestrates the entire process. — location: [4437](kindle://book?action=open&asin=B0B2DPFJN4&location=4437) ^ref-54237

---
With no coordinator to tell them what to do, each participant listens for the events that signal their turn. The coordination logic is spread out across the components and is not centralized. — location: [4442](kindle://book?action=open&asin=B0B2DPFJN4&location=4442) ^ref-3341

---
Using a choreographed saga is a good choice when the number of participants is low, and the coordination logic is easy to follow. Choreography makes use of the events that participants already publish and subscribe to and does not need any extra services or processes to be deployed. — location: [4487](kindle://book?action=open&asin=B0B2DPFJN4&location=4487) ^ref-7578

---
An orchestrated saga does not rely on individual components publishing events. Instead, it uses a saga execution coordinator (SEC) to send commands to the components. — location: [4491](kindle://book?action=open&asin=B0B2DPFJN4&location=4491) ^ref-9685

---

---
kindle-sync:
  bookId: '38140'
  title: Implementing Domain-Driven Design
  author: Vernon Vaughn
  asin: B00BCLEBN8
  lastAnnotatedDate: '2023-08-27'
  bookImageUrl: 'https://m.media-amazon.com/images/I/91R339O1AZL._SY160.jpg'
  highlightsCount: 119
---
# Implementing Domain-Driven Design
## Metadata
* Author: [Vernon Vaughn](https://www.amazon.comundefined)
* ASIN: B00BCLEBN8
* Reference: https://www.amazon.com/dp/B00BCLEBN8
* [Kindle link](kindle://book?action=open&asin=B00BCLEBN8)

## Highlights
When implemented correctly, DDD helps us reach the point where our design is exactly how the software works. — location: [661](kindle://book?action=open&asin=B00BCLEBN8&location=661) ^ref-32590

---
models are developed in Bounded Contexts. — location: [1507](kindle://book?action=open&asin=B00BCLEBN8&location=1507) ^ref-7041

---
four primary Subdomains: Product Catalog, Orders, Invoicing, and Shipping. — location: [1519](kindle://book?action=open&asin=B00BCLEBN8&location=1519) ^ref-10946

---
Domain is a part of the business Domain that is of primary importance to the success of the organization. — location: [1642](kindle://book?action=open&asin=B00BCLEBN8&location=1642) ^ref-40410

---
The problem space enables us to think of a strategic business challenge to be solved, while the solution space focuses on how we will implement the software to solve the problem of the business challenge. — location: [1747](kindle://book?action=open&asin=B00BCLEBN8&location=1747) ^ref-57500

---
The solution space is one or more Bounded Contexts, a set of specific software models. — location: [1755](kindle://book?action=open&asin=B00BCLEBN8&location=1755) ^ref-61381

---
It is a desirable goal to align Subdomains one-to-one with Bounded Contexts. — location: [1757](kindle://book?action=open&asin=B00BCLEBN8&location=1757) ^ref-49163

---
we rigorously separate the various concerns of our application or system into well-defined layers. — location: [2915](kindle://book?action=open&asin=B00BCLEBN8&location=2915) ^ref-22119

---
An essential rule of this architecture is that each layer may couple only to itself and below. — location: [2923](kindle://book?action=open&asin=B00BCLEBN8&location=2923) ^ref-39601

---
A Strict Layers Architecture is one that allows coupling only to the layer directly below. A Relaxed Layers Architecture, however, allows any higher-level layer to couple to any layer below it. — location: [2924](kindle://book?action=open&asin=B00BCLEBN8&location=2924) ^ref-48571

---
Lower layers may actually loosely couple to higher layers, but this is only by means of a mechanism such as Observer or Mediator [Gamma et al.]; there is never a direct reference from lower to higher. — location: [2927](kindle://book?action=open&asin=B00BCLEBN8&location=2927) ^ref-32283

---
Using Mediator, for example, the higher layer would implement an interface defined by the lower layer, then pass the implementing object as an argument to the lower layer. The lower layer uses the implementing object with no knowledge of where it resides architecturally. — location: [2929](kindle://book?action=open&asin=B00BCLEBN8&location=2929) ^ref-28082

---
we still want to limit coarse-grained validations that express deep business knowledge only to the model. — location: [2933](kindle://book?action=open&asin=B00BCLEBN8&location=2933) ^ref-29331

---
Application Services (14) reside in the Application Layer. These are different from Domain Services (7) and are thus devoid of domain logic. — location: [2939](kindle://book?action=open&asin=B00BCLEBN8&location=2939) ^ref-19270

---
They may control persistence transactions and security. They may also be in charge of sending Event-based notifications to other systems and/or — location: [2940](kindle://book?action=open&asin=B00BCLEBN8&location=2940) ^ref-17899

---
The Application Services in this layer are the direct clients of the domain model, though themselves possessing no business logic. — location: [2942](kindle://book?action=open&asin=B00BCLEBN8&location=2942) ^ref-55240

---
a common function of an Application Service is to accept parameters from the User Interface, use a Repository (12) to obtain an Aggregate instance, and then execute some command operation on it: — location: [2944](kindle://book?action=open&asin=B00BCLEBN8&location=2944) ^ref-64473

---
If our Application Services become much more complex than this, it is probably an indication that domain logic is leaking into the Application Services, and that the model is becoming anemic. So — location: [2953](kindle://book?action=open&asin=B00BCLEBN8&location=2953) ^ref-46715

---
When a new Aggregate must be created, an Application Service would use a Factory (11) or the Aggregate’s constructor — location: [2955](kindle://book?action=open&asin=B00BCLEBN8&location=2955) ^ref-41176

---
When the domain model is designed to publish Domain Events (8), the Application Layer may register subscribers to any number of Events. — location: [2957](kindle://book?action=open&asin=B00BCLEBN8&location=2957) ^ref-33177

---
Using Layers may require the Domain Layer to make some limited use of Infrastructure. — location: [2962](kindle://book?action=open&asin=B00BCLEBN8&location=2962) ^ref-38141

---
definition of Layers may require implementations of some interfaces in the Domain Layer that depend on technologies provided by Infrastructure. — location: [2964](kindle://book?action=open&asin=B00BCLEBN8&location=2964) ^ref-28548

---
we want to reject any notion of coupling core domain model objects to Infrastructure. — location: [2981](kindle://book?action=open&asin=B00BCLEBN8&location=2981) ^ref-44024

---
High-level modules should not depend on low-level modules. Both should depend on abstractions. — location: [2989](kindle://book?action=open&asin=B00BCLEBN8&location=2989) ^ref-13104

---
Abstractions should not depend upon details. Details should depend upon abstractions. — location: [2990](kindle://book?action=open&asin=B00BCLEBN8&location=2990) ^ref-19317

---
The possible Layers when the Dependency Inversion Principle is used. — location: [2995](kindle://book?action=open&asin=B00BCLEBN8&location=2995) ^ref-11995

---
we would have a Repository implemented in Infrastructure for an interface defined in Domain: — location: [3003](kindle://book?action=open&asin=B00BCLEBN8&location=3003) ^ref-10681

---
Focusing on the Domain Layer, using DIP enables both the Domain and Infrastructure to depend on abstractions (interfaces) defined by the domain model. — location: [3015](kindle://book?action=open&asin=B00BCLEBN8&location=3015) ^ref-33119

---
It may use any one of a few ways to acquire the implementations, including Dependency Injection, Service Factory, and Plug In — location: [3018](kindle://book?action=open&asin=B00BCLEBN8&location=3018) ^ref-60442

---
Need a new client? Not a problem. Just add an Adapter to transform any given client’s input into that understood by the internal application’s API. — location: [3028](kindle://book?action=open&asin=B00BCLEBN8&location=3028) ^ref-37248

---
output mechanisms employed by the system, such as graphics, persistence, and messaging, may also be diverse and swappable. — location: [3029](kindle://book?action=open&asin=B00BCLEBN8&location=3029) ^ref-14899

---
That’s possible because an Adapter is created to transform application results into a form accepted by a specific output mechanism. — location: [3030](kindle://book?action=open&asin=B00BCLEBN8&location=3030) ^ref-63953

---
It’s just that it encourages a way of producing an architecture that leans naturally toward the development of a Ports and Adapters style. — location: [3034](kindle://book?action=open&asin=B00BCLEBN8&location=3034) ^ref-54861

---
The outside enables disparate clients to submit input and also provides mechanisms to retrieve persisted data, store the application’s output (for example, a database), or send it elsewhere along its way (for example, messaging). — location: [3039](kindle://book?action=open&asin=B00BCLEBN8&location=3039) ^ref-8521

---
client requests arrive and the respective Adapter transforms their input. It then invokes an operation on the application or sends the application an event. Control is thus transferred to the inside. — location: [3051](kindle://book?action=open&asin=B00BCLEBN8&location=3051) ^ref-28868

---
We Probably Are Not Implementing the Ports Ourselves — location: [3053](kindle://book?action=open&asin=B00BCLEBN8&location=3053) ^ref-64286

---
Design the Application Inside per Functional Requirements — location: [3059](kindle://book?action=open&asin=B00BCLEBN8&location=3059) ^ref-54591

---
When using Hexagonal, we design the application with our use cases in mind, not the number of supported clients. — location: [3059](kindle://book?action=open&asin=B00BCLEBN8&location=3059) ^ref-8286

---
Now think of segregating all of the pure query responsibilities traditionally found in a model from all responsibilities that execute pure commands on the same model. — location: [3292](kindle://book?action=open&asin=B00BCLEBN8&location=3292) ^ref-38797

---
We still need a way to display data to the user. For that we create a second model, one that is tuned for optimized queries. That’s our query model. — location: [3298](kindle://book?action=open&asin=B00BCLEBN8&location=3298) ^ref-21008

---
Instead of designing domain concepts with rich behaviors, we might think primarily about the attributes (columns) and associations (foreign keys) of the data. — location: [3882](kindle://book?action=open&asin=B00BCLEBN8&location=3882) ^ref-10896

---
We design a domain concept as an Entity when we care about its individuality, when distinguishing it from all other objects in a system is a mandatory constraint. — location: [3894](kindle://book?action=open&asin=B00BCLEBN8&location=3894) ^ref-10243

---
unique identity and mutability characteristics that set Entities apart from Value Objects (6). — location: [3900](kindle://book?action=open&asin=B00BCLEBN8&location=3900) ^ref-13633

---
It is quite possible that a CRUD-based system would be more fitting. — location: [3903](kindle://book?action=open&asin=B00BCLEBN8&location=3903) ^ref-42260

---
Rather than focusing on the attributes or even the behavior, strip the Entity object’s definition down to the most intrinsic characteristics, particularly those that identify it or are commonly used to find or match it. — location: [3924](kindle://book?action=open&asin=B00BCLEBN8&location=3924) ^ref-8873

---
Value Objects can serve as holders of unique identity. They are immutable, — location: [3934](kindle://book?action=open&asin=B00BCLEBN8&location=3934) ^ref-14976

---
For higher-performance domains we can cache any number of UUID instances, refilling the cache in the background. If cached UUID instances are lost due to server restart, there are no gaps in identities because they are all based on random, manufactured values. Refilling the cache on server restart has no negative consequences of abandoned values. — location: [4001](kindle://book?action=open&asin=B00BCLEBN8&location=4001) ^ref-54806

---
A full UUID is usually appropriate when it can be hidden from users and human-readable reference techniques can be used. — location: [4009](kindle://book?action=open&asin=B00BCLEBN8&location=4009) ^ref-11820

---
the Entity serving as an Aggregate Root requires global unique identity. — location: [4016](kindle://book?action=open&asin=B00BCLEBN8&location=4016) ^ref-2389

---
One possible downside is performance. It can take significantly longer to go to the database to get each value than to generate identities in the application. — location: [4057](kindle://book?action=open&asin=B00BCLEBN8&location=4057) ^ref-40557

---
Early identity generation and assignment happen before the Entity is persisted. — location: [4076](kindle://book?action=open&asin=B00BCLEBN8&location=4076) ^ref-36135

---
Late identity generation and assignment happen when the Entity is persisted. — location: [4077](kindle://book?action=open&asin=B00BCLEBN8&location=4077) ^ref-64493

---
We’ve created a table in a MySQL database named product_seq. Next, we insert a single row into the table, initializing its one and only column, nextval, to 0. — location: [4098](kindle://book?action=open&asin=B00BCLEBN8&location=4098) ^ref-28045

---
We update the one and only row by incrementing the nextval column by 1. The update statement uses a MySQL function, LAST_INSERT_ID(), to increment the column’s INT value. The expression parameter is first executed, then the result is assigned to the nextval column. The result of the expression parameter nextval + 1 remains stable in the LAST_INSERT_ID() function, such that when the subsequence SELECT LAST_INSERT_ID() statement is evaluated, the value of nextval that results from that exact execution is returned in the result set. — location: [4102](kindle://book?action=open&asin=B00BCLEBN8&location=4102) ^ref-54418

---
identity of the selected choice is used as the local identity. Some additional state (properties) from the foreign Entity may also be copied into the local Entity. — location: [4151](kindle://book?action=open&asin=B00BCLEBN8&location=4151) ^ref-8446

---
Our local Bounded Context subscribes to Domain Events published by external systems. When a relevant notification is received, our local system transitions its own Aggregate Entities to reflect the state of those in external systems. — location: [4157](kindle://book?action=open&asin=B00BCLEBN8&location=4157) ^ref-38184

---
When autonomy is achieved, it can actually narrow searches to local objects. This is not a matter of caching foreign objects locally. Rather, it involves translating foreign concepts into those of the local Bounded Context, as explained in Context Mapping (3). — location: [4160](kindle://book?action=open&asin=B00BCLEBN8&location=4160) ^ref-56477

---
This is the most complex of identity creation strategies. The maintenance of the local Entity is dependent not only on transitions caused by local domain behaviors but possibly also on those that occur in one or more external systems. — location: [4162](kindle://book?action=open&asin=B00BCLEBN8&location=4162) ^ref-56463

---
There is another problem that can occur when identity generation is delayed until the Entity is persisted. It occurs when two or more new Entities must be added to a java.util.Set, but their identity has not yet been assigned, making them equal to the other new ones — location: [4186](kindle://book?action=open&asin=B00BCLEBN8&location=4186) ^ref-42196

---
To avoid this bug we must do one of two things. Either we change the design to allocate and assign identity early, or we refactor the equals() method to compare attributes other than the domain identity. — location: [4193](kindle://book?action=open&asin=B00BCLEBN8&location=4193) ^ref-41259

---
In most cases unique identity must be protected from modification, remaining stable throughout the lifetime of the Entity to which it is assigned. — location: [4274](kindle://book?action=open&asin=B00BCLEBN8&location=4274) ^ref-59596

---
We might also create guards in setters to prevent even the Entity itself from changing the state of the identity if it already exists. — location: [4276](kindle://book?action=open&asin=B00BCLEBN8&location=4276) ^ref-44219

---
Some terminology uncovered will be nouns that name things, adjectives that describe them, and verbs that indicate what the things do. — location: [4332](kindle://book?action=open&asin=B00BCLEBN8&location=4332) ^ref-43614

---
Yes, there is a Tenant Entity, and no, this doesn’t mean there is not a User Entity. They are both Entities. To understand why Tenant and User are the Roots (10) of two different Aggregates, — location: [4361](kindle://book?action=open&asin=B00BCLEBN8&location=4361) ^ref-22950

---
The justification here is that each User must be uniquely identified, clearly distinguished from all others. A User must also support change over time, so it is clearly an Entity. — location: [4367](kindle://book?action=open&asin=B00BCLEBN8&location=4367) ^ref-50256

---
important to state that tenants may be active or inactive, and that users can be authenticated only when their tenancy is active. — location: [4382](kindle://book?action=open&asin=B00BCLEBN8&location=4382) ^ref-15555

---
The question is, Should this identity have a specialized type, or can it remain a simple String? — location: [4402](kindle://book?action=open&asin=B00BCLEBN8&location=4402) ^ref-60482

---
By defining a TenantId Value Object, the team could more confidently ensure that all subscriber-owned Entities were striped with the correct identity. — location: [4405](kindle://book?action=open&asin=B00BCLEBN8&location=4405) ^ref-9812

---
The Tenant must be named. The name can be a simple String attribute because it has no special behavior. — location: [4411](kindle://book?action=open&asin=B00BCLEBN8&location=4411) ^ref-3409

---
Since they will need a way to encrypt each password before it is associated with the User, it seemed as if this called for some kind of Domain Service (7). — location: [4436](kindle://book?action=open&asin=B00BCLEBN8&location=4436) ^ref-23662

---
Encryption Service: Provides a means to encrypt passwords and other data that cannot be stored and used as clear text. — location: [4443](kindle://book?action=open&asin=B00BCLEBN8&location=4443) ^ref-43485

---
If we were to place active in the attributes compartment of Tenant in the class diagram, would that necessarily tell the reader anything useful? — location: [4465](kindle://book?action=open&asin=B00BCLEBN8&location=4465) ^ref-38022

---
the team noted that domain experts talk about activating and deactivating. To incorporate that terminology they’d assign operations such as activate() and deactivate() instead. — location: [4477](kindle://book?action=open&asin=B00BCLEBN8&location=4477) ^ref-53584

---
Writing the test made them realize that another method, isActive(), was needed. — location: [4494](kindle://book?action=open&asin=B00BCLEBN8&location=4494) ^ref-52660

---
Ubiquitous Language glossary grew as well: — location: [4495](kindle://book?action=open&asin=B00BCLEBN8&location=4495) ^ref-22329

---
Since there is more to authentication than merely finding a User that matches a specific username and password, a higher-level coordinator is needed. Domain Services are good at that. — location: [4508](kindle://book?action=open&asin=B00BCLEBN8&location=4508) ^ref-12679

---
Person is modeled as a separate class to avoid placing too much responsibility on the User. — location: [4529](kindle://book?action=open&asin=B00BCLEBN8&location=4529) ^ref-63692

---
Should clients be given access to the Person object inside the User? — location: [4542](kindle://book?action=open&asin=B00BCLEBN8&location=4542) ^ref-38713

---
One developer questioned whether a User would always be a person. — location: [4544](kindle://book?action=open&asin=B00BCLEBN8&location=4544) ^ref-54625

---
If clients were given access to the shape of User, with navigation into the Person in order to execute behavior, that could require client refactoring later. — location: [4545](kindle://book?action=open&asin=B00BCLEBN8&location=4545) ^ref-29743

---
The accessor could later be redesigned to serve a Principal interface, and Person and System would each be a specialized Principal. The team would be able to refactor this as they gained deeper understanding. — location: [4554](kindle://book?action=open&asin=B00BCLEBN8&location=4554) ^ref-21129

---
Access to even the encrypted password is never granted to clients. Once the password is set on User, it is never exposed beyond the Aggregate boundary. — location: [4562](kindle://book?action=open&asin=B00BCLEBN8&location=4562) ^ref-36821

---
Anything seeking authentication has but one approach, using the AuthenticationService. — location: [4563](kindle://book?action=open&asin=B00BCLEBN8&location=4563) ^ref-26642

---
Events would accomplish at least two things. First, they would enable change tracking through the life cycle of all objects (discussed later). Second, they would enable outside subscribers to synchronize with the changes, giving outsiders the potential for autonomy. — location: [4566](kindle://book?action=open&asin=B00BCLEBN8&location=4566) ^ref-41547

---
An aspect of modeling is to discover the roles and responsibilities of objects. — location: [4570](kindle://book?action=open&asin=B00BCLEBN8&location=4570) ^ref-63612

---
An invariant is a business rule that must always be consistent. — location: [8037](kindle://book?action=open&asin=B00BCLEBN8&location=8037) ^ref-45469

---
When you store something in a repository and later return to retrieve it, you expect that it will be in the same state as it was in when you put it there. — location: [9066](kindle://book?action=open&asin=B00BCLEBN8&location=9066) ^ref-6183

---
For each type of object that needs global access, create an object that can provide the illusion of an in-memory collection of all objects of that type. Set up access through a well-known global interface. — location: [9071](kindle://book?action=open&asin=B00BCLEBN8&location=9071) ^ref-32451

---
Provide repositories only for aggregates. — location: [9074](kindle://book?action=open&asin=B00BCLEBN8&location=9074) ^ref-39426

---
Every persistent Aggregate type will have a Repository. — location: [9075](kindle://book?action=open&asin=B00BCLEBN8&location=9075) ^ref-33573

---
Generally speaking, there is a one-to-one relationship between an Aggregate type and a Repository. However, sometimes when two or more Aggregate types share an object hierarchy, the types may share a single Repository. — location: [9076](kindle://book?action=open&asin=B00BCLEBN8&location=9076) ^ref-40961

---
there are two kinds of Repository designs, a collection-oriented design and a persistence-oriented design. — location: [9093](kindle://book?action=open&asin=B00BCLEBN8&location=9093) ^ref-58830

---
These very closely mimic a collection, simulating at least some of its standard interface. Here you design a Repository interface that does not hint in any way that there is an underlying persistence mechanism, avoiding any notion of saving or persisting data to a store. — location: [9097](kindle://book?action=open&asin=B00BCLEBN8&location=9097) ^ref-4513

---
If we add the Aggregate instance calendar to a CalendarRepository designed with a collection orientation, adding calendar a second time is benign. Each Aggregate has a globally unique identity that is associated with the Root Entity (5, 10). It is this unique identity that allows the Set-like Repository to prevent adding the same Aggregate instances more than once. — location: [9132](kindle://book?action=open&asin=B00BCLEBN8&location=9132) ^ref-34462

---
Whatever the backing implementation with a specific persistence mechanism, you must not allow instances of the same object to be added twice. — location: [9138](kindle://book?action=open&asin=B00BCLEBN8&location=9138) ^ref-5008

---
Another key takeaway is that you don’t need to “re-save” modified objects already held by the Repository. — location: [9139](kindle://book?action=open&asin=B00BCLEBN8&location=9139) ^ref-22745

---
A Repository should mimic a Set collection. — location: [9143](kindle://book?action=open&asin=B00BCLEBN8&location=9143) ^ref-27958

---
when retrieving objects from a Repository and modifying them, you don’t need to “re-save” them to the Repository. — location: [9145](kindle://book?action=open&asin=B00BCLEBN8&location=9145) ^ref-46094

---
CalendarRepository doesn’t have a save() method because there is no need for one. — location: [9172](kindle://book?action=open&asin=B00BCLEBN8&location=9172) ^ref-4931

---
The bottom line, then, is that a traditional collection-oriented Repository truly mimics a collection in that no parts of the persistence mechanisms are surfaced to the client by its public interface. — location: [9176](kindle://book?action=open&asin=B00BCLEBN8&location=9176) ^ref-4509

---
the overall advantage to either of these approaches is that persistent object changes are tracked implicitly, requiring no explicit client knowledge or intervention to make changes known to the persistence mechanism. — location: [9195](kindle://book?action=open&asin=B00BCLEBN8&location=9195) ^ref-21415

---
Place the interface definition in the same Module (9) as the Aggregate type that it stores. — location: [9223](kindle://book?action=open&asin=B00BCLEBN8&location=9223) ^ref-54216

---
The implementation class goes in a separate package, as discussed later. — location: [9225](kindle://book?action=open&asin=B00BCLEBN8&location=9225) ^ref-52907

---
Thus, void may be the more accurate return type in the case of a Repository. — location: [9236](kindle://book?action=open&asin=B00BCLEBN8&location=9236) ^ref-15009

---
you may determine not to include any removal methods on the Repository public interface, or you may decide to implement the removal methods to set the unusable state of the Aggregate instance. — location: [9249](kindle://book?action=open&asin=B00BCLEBN8&location=9249) ^ref-42136

---
Another important part of the Repository interface is the definition of finder methods: — location: [9254](kindle://book?action=open&asin=B00BCLEBN8&location=9254) ^ref-43023

---
Some like to use a Module (Java package) directly under the Aggregate and Repository Module. In this case that would mean — location: [9288](kindle://book?action=open&asin=B00BCLEBN8&location=9288) ^ref-42544

---
Placing the class here allows you to manage the implementation in the Domain Layer, but in a special package for implementations. — location: [9293](kindle://book?action=open&asin=B00BCLEBN8&location=9293) ^ref-21953

---
Adding can cause a ConstraintViolationException. Rather than allowing Hibernate exceptions to trickle out to clients, those exceptions are caught and wrapped by the more client-friendly IllegalStateException. We could also declare domain-specific exceptions and throw those. — location: [9354](kindle://book?action=open&asin=B00BCLEBN8&location=9354) ^ref-65243

---
The inner Person object must first be deleted, and then the User Aggregate Root. If you do not delete the inner Person object, it will be orphaned in — location: [9373](kindle://book?action=open&asin=B00BCLEBN8&location=9373) ^ref-32533

---
DDD experts avoid Aggregate-managed persistence as a rule of thumb. — location: [9381](kindle://book?action=open&asin=B00BCLEBN8&location=9381) ^ref-6616

---
method registerObject() answers a clone of the original Calendar instance. It is this clone object, referenced by calendarToRename, that must be edited/modified. As you cause modifications on the object, TopLink is able to track the changes that occur. When method commit() on UnitOfWork is invoked, all modified objects are committed to the database. — location: [9440](kindle://book?action=open&asin=B00BCLEBN8&location=9440) ^ref-15482

---
To reiterate, when using a collection-oriented style, Aggregate instances are added only when they are created. When using a persistence-oriented style, Aggregate instances must be saved both when they are created and when they are modified: — location: [9540](kindle://book?action=open&asin=B00BCLEBN8&location=9540) ^ref-44074

---
The domain model and its encompassing Domain Layer is never the correct place to manage transactions. — location: [9857](kindle://book?action=open&asin=B00BCLEBN8&location=9857) ^ref-8629

---
an object-relational mapping tool also provides an abstraction over a persistence mechanism, but it is neither a Repository nor a DAO. — location: [10040](kindle://book?action=open&asin=B00BCLEBN8&location=10040) ^ref-10214

---
a DAO is expressed in terms of database tables, providing CRUD interfaces to them. — location: [10043](kindle://book?action=open&asin=B00BCLEBN8&location=10043) ^ref-58136

---
The user interface will make use of application-level services that coordinate use case tasks, manage transactions, and assert necessary security authorizations. — location: [11837](kindle://book?action=open&asin=B00BCLEBN8&location=11837) ^ref-53025

---
When a model exists to support another model, the supporting model may be as simple as a set of classes in a separate Module (9) that address a specialty concept and provide some algorithms. — location: [11851](kindle://book?action=open&asin=B00BCLEBN8&location=11851) ^ref-38731

---
when an application depends on other applications or services through integration, the whole solution could be called a system. — location: [11856](kindle://book?action=open&asin=B00BCLEBN8&location=11856) ^ref-7639

---

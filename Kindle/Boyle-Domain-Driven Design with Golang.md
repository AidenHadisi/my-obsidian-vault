---
kindle-sync:
  bookId: '25284'
  title: >-
    Domain-Driven Design with Golang: Use Golang to create simple, maintainable
    systems to solve complex business problems
  author: Matthew Boyle
  asin: B0BNJ8KHYN
  lastAnnotatedDate: '2023-06-27'
  bookImageUrl: 'https://m.media-amazon.com/images/I/71RllhJ7eqL._SY160.jpg'
  highlightsCount: 187
---
# Domain-Driven Design with Golang
## Metadata
* Author: [Matthew Boyle](https://www.amazon.comundefined)
* ASIN: B0BNJ8KHYN
* Reference: https://www.amazon.com/dp/B0BNJ8KHYN
* [Kindle link](kindle://book?action=open&asin=B0BNJ8KHYN)

## Highlights
Given this definition, the AddUser function now doesn’t seem like such a good idea. — location: [576](kindle://book?action=open&asin=B0BNJ8KHYN&location=576) ^ref-15902

---
we go back to the brief, we see that someone new to the app is called a lead, and once they select a subscription, they convert into a customer. Given this, we can make some amendments to our code, as follows: — location: [579](kindle://book?action=open&asin=B0BNJ8KHYN&location=579) ^ref-57487

---
type LeadCreator interface — location: [583](kindle://book?action=open&asin=B0BNJ8KHYN&location=583) ^ref-26179

---
type LeadConvertor interface — location: [585](kindle://book?action=open&asin=B0BNJ8KHYN&location=585) ^ref-32310

---
Evans advises that ubiquitous language should only apply to a single bounded context — location: [598](kindle://book?action=open&asin=B0BNJ8KHYN&location=598) ^ref-2078

---
Bounded contexts are all about dividing large models into smaller, easier-to-understand chunks and being explicit about how they relate to each other. — location: [607](kindle://book?action=open&asin=B0BNJ8KHYN&location=607) ^ref-56039

---
An Open Host Service is a means of giving other systems (or sub-systems) access to ours. Evans — location: [627](kindle://book?action=open&asin=B0BNJ8KHYN&location=627) ^ref-48480

---
type UserHandler interface {     IsUserSubscriptionActive(ctx context.Context, userID string) bool } — location: [642](kindle://book?action=open&asin=B0BNJ8KHYN&location=642) ^ref-14825

---
Two popular ways to present published language are via OpenAPI or gRPC. — location: [662](kindle://book?action=open&asin=B0BNJ8KHYN&location=662) ^ref-54690

---
We can use OpenAPI to define the schema. This — location: [664](kindle://book?action=open&asin=B0BNJ8KHYN&location=664) ^ref-39997

---
You can use a tool called Swagger for this. — location: [666](kindle://book?action=open&asin=B0BNJ8KHYN&location=666) ^ref-44428

---
If you want to play around and generate your own OpenAPI code from a specification, you can use the Swagger Editor (https://editor.swagger.io) in your browser. — location: [693](kindle://book?action=open&asin=B0BNJ8KHYN&location=693) ^ref-6975

---
You now have an interface for a server that you can implement. Every time you update your API documentation, you can rerun this command to generate a new server definition. — location: [725](kindle://book?action=open&asin=B0BNJ8KHYN&location=725) ^ref-24238

---
Again, if we updated our OpenAPI specification and wanted to update the client, all we would need to do is run the preceding command again. You could set up a job as part of your continuous integration (CI) pipeline that generates a new client package every time a specification change is made, allowing consumer teams to get the latest version whenever they need it. — location: [734](kindle://book?action=open&asin=B0BNJ8KHYN&location=734) ^ref-15124

---
gRPC was created at Google to handle remote communication at scale. It supports load balancing, tracing, health checks, bi-directional streaming, and authentication. — location: [749](kindle://book?action=open&asin=B0BNJ8KHYN&location=749) ^ref-42774

---
gRPC uses binary serialization to compress the payload it sends, making it very efficient and fast. — location: [752](kindle://book?action=open&asin=B0BNJ8KHYN&location=752) ^ref-43497

---
To call a method on a remote server, firstly, we must define our message protobuf. — location: [758](kindle://book?action=open&asin=B0BNJ8KHYN&location=758) ^ref-16878

---
We are going to use buf (https://buf.build) to generate our Go client and server — location: [781](kindle://book?action=open&asin=B0BNJ8KHYN&location=781) ^ref-53643

---
Sometimes called an adapter layer, an anti-corruption layer can be used to translate models from different systems. — location: [839](kindle://book?action=open&asin=B0BNJ8KHYN&location=839) ^ref-46089

---
care about most of the same information, but we name it differently or have a slightly different format. We have two options here: We can swap our campaign model to be exactly the same as the marketing model. This would go against the principles of DDD and mean we are strongly coupling the domain model to something outside of our control. We can write an anti-corruption layer. — location: [850](kindle://book?action=open&asin=B0BNJ8KHYN&location=850) ^ref-4324

---
func (m *MarketingCampaignModel) ToCampaign() (*Campaign, error) { — location: [862](kindle://book?action=open&asin=B0BNJ8KHYN&location=862) ^ref-45694

---
Of all the DDD patterns, the anti-corruption pattern is the one I use most when working on systems that do not use DDD. It’s simple but very effective for ensuring we keep systems decoupled. — location: [877](kindle://book?action=open&asin=B0BNJ8KHYN&location=877) ^ref-2989

---
We will finish by looking at aggregates, which are useful when we need to cluster domain objects together and treat them as a single item. — location: [897](kindle://book?action=open&asin=B0BNJ8KHYN&location=897) ^ref-64375

---
In domain-driven design, entities are defined by their identity. Their attributes do not define them, and it is expected that although their attributes may change over time, their identity will not. — location: [918](kindle://book?action=open&asin=B0BNJ8KHYN&location=918) ^ref-62249

---
These actions do not change the identity of our entity. We are still referencing the same ID, — location: [928](kindle://book?action=open&asin=B0BNJ8KHYN&location=928) ^ref-61946

---
Entity IDs do not necessarily have to be generated by the system. They may form part of the entity’s attributes. — location: [938](kindle://book?action=open&asin=B0BNJ8KHYN&location=938) ^ref-60188

---
email addresses would be much better suited to be an attribute of the entity. — location: [943](kindle://book?action=open&asin=B0BNJ8KHYN&location=943) ^ref-11107

---
It is essential to try and future-proof your system as much as possible, especially when it comes to things such as entity identifiers. — location: [957](kindle://book?action=open&asin=B0BNJ8KHYN&location=957) ^ref-1109

---
If you are using a persistent store such as PostgreSQL, you can lean on it to create a UUID for you. — location: [965](kindle://book?action=open&asin=B0BNJ8KHYN&location=965) ^ref-54334

---
Anemic models have little or no domain behavior as part of their design. This means that you are not getting the full benefit of DDD. — location: [971](kindle://book?action=open&asin=B0BNJ8KHYN&location=971) ^ref-7762

---
If your model has mostly public getter and setter functions, no business logic, or depends on various clients to implement the business logic, you probably have an anemic model. — location: [973](kindle://book?action=open&asin=B0BNJ8KHYN&location=973) ^ref-43960

---
func (a *AuctionRefactored) GetAuctionElapsedDuration() time.Duration {    return a.auctionStart.Sub(a.auctionEnd) } — location: [997](kindle://book?action=open&asin=B0BNJ8KHYN&location=997) ^ref-7875

---
am not a fan of ORMs – they lead to a layer of unnecessary abstraction and poor database query design, which is often one of the biggest reasons applications have performance issues. — location: [1019](kindle://book?action=open&asin=B0BNJ8KHYN&location=1019) ^ref-11394

---
By using an ORM, you are delegating control of query creation and planning. — location: [1021](kindle://book?action=open&asin=B0BNJ8KHYN&location=1021) ^ref-63399

---
If you want to use an ORM, ensure it does not control how you write your entities in your DDD context; otherwise, you may end up with an anemic model. We also want to keep the coupling between our entity and ORM to a minimum. Therefore, I recommend you use an adaptor layer to decouple your ORM and DDD entity layer. — location: [1021](kindle://book?action=open&asin=B0BNJ8KHYN&location=1021) ^ref-60990

---
Value objects are, in some ways, the opposite of entities. With value objects, we want to assert that two objects are the same given their values. — location: [1026](kindle://book?action=open&asin=B0BNJ8KHYN&location=1026) ^ref-13144

---
We typically use them to measure, quantify, or describe something about our domain. — location: [1029](kindle://book?action=open&asin=B0BNJ8KHYN&location=1029) ^ref-17397

---
Notice how, in the point class, x and y are lowercase? This is to stop them from being exported and mutated. It is recommended that value objects remain immutable to prevent any unexpected behavior. — location: [1052](kindle://book?action=open&asin=B0BNJ8KHYN&location=1052) ^ref-4798

---
We should aim to use value objects as much as possible when modeling our domain. This is because they are the safest constructs we can use when implemented correctly. — location: [1075](kindle://book?action=open&asin=B0BNJ8KHYN&location=1075) ^ref-34412

---
If you care only about the values of an object, then it should preferably be a value object. — location: [1078](kindle://book?action=open&asin=B0BNJ8KHYN&location=1078) ^ref-2350

---
Some other questions to ask yourself to ensure a value object is the right choice for you are: Is it possible for me to treat this object as immutable? Does it measure, quantify, or describe a domain concept? Can it be compared to other objects of the same type by its values? — location: [1078](kindle://book?action=open&asin=B0BNJ8KHYN&location=1078) ^ref-61039

---
Try and make everything a value object to start with until it does not fit your use case. At that point, it can be upgraded to an entity. — location: [1084](kindle://book?action=open&asin=B0BNJ8KHYN&location=1084) ^ref-32369

---
In domain-driven design, the aggregate pattern refers to a group of domain objects that can be treated as one for some behaviors. — location: [1091](kindle://book?action=open&asin=B0BNJ8KHYN&location=1091) ^ref-61475

---
An order: Typically, an order consists of individual items, but it is helpful to treat them as a single thing (an order) for some purposes within our system. — location: [1093](kindle://book?action=open&asin=B0BNJ8KHYN&location=1093) ^ref-27996

---
team: A team consists of many employees. In our system, we would likely have a domain object for employees, but grouping them and applying behaviors to them as a team would be helpful in situations such as organizing departments. — location: [1095](kindle://book?action=open&asin=B0BNJ8KHYN&location=1095) ^ref-42386

---
Instead, the job of an aggregate pattern is to act as a transaction boundary for the domain objects within. — location: [1104](kindle://book?action=open&asin=B0BNJ8KHYN&location=1104) ^ref-48929

---
Loading, saving, editing, and deleting should happen to all objects within the aggregate or not at all. — location: [1105](kindle://book?action=open&asin=B0BNJ8KHYN&location=1105) ^ref-35180

---
If an order is canceled, we should return all items within that order to stock. We may also want to trigger a refund. — location: [1106](kindle://book?action=open&asin=B0BNJ8KHYN&location=1106) ^ref-14156

---
An invariant is simply a rule in our domain that must always be true. For example, we may say that in our system, for an order to be created, we must have the item in stock. This is a business invariant. If we do not have an item in stock, we cannot promise it to customers. — location: [1128](kindle://book?action=open&asin=B0BNJ8KHYN&location=1128) ^ref-49465

---
For aggregates, we are looking for transactional consistency, not eventual consistency; we want any changes to our aggregate to be immediate and atomic. Therefore, we can think of an aggregate as a transactional consistency boundary. Whenever we make changes within our domain, we should ideally only modify one aggregate per transaction. If it is more, then your model is probably not quite correct, and you should revisit it. — location: [1130](kindle://book?action=open&asin=B0BNJ8KHYN&location=1130) ^ref-49601

---
Generally, we should aim for small aggregates. Keeping aggregates small will help make our system more scalable, improve performance, and give transactions more chance of success. — location: [1134](kindle://book?action=open&asin=B0BNJ8KHYN&location=1134) ^ref-13193

---
Firstly, from a bounded context perspective, marketing opt-in has nothing to do with the order object. — location: [1144](kindle://book?action=open&asin=B0BNJ8KHYN&location=1144) ^ref-11727

---
Secondly, if a user were to opt out of marketing between starting an order and completing it, we would not want the order to not complete. Therefore, removing it from our aggregate makes sense: — location: [1145](kindle://book?action=open&asin=B0BNJ8KHYN&location=1145) ^ref-3809

---
This means we expect the other systems to receive and process our event in a reasonable amount of time, but we do not expect it to be atomically up-to-date as we would expect our bounded contexts to be. This leads to more decoupled systems with stronger resilience and scalability possibilities. — location: [1160](kindle://book?action=open&asin=B0BNJ8KHYN&location=1160) ^ref-54882

---
The factory pattern is typically used in object-oriented programming and is defined as an object with the primary responsibility of creating other objects. — location: [1203](kindle://book?action=open&asin=B0BNJ8KHYN&location=1203) ^ref-39526

---
Typically, factory classes should have no other purpose than object creation. — location: [1214](kindle://book?action=open&asin=B0BNJ8KHYN&location=1214) ^ref-25903

---
Repositories are the parts of our code that contain the logic necessary to access data sources. — location: [1257](kindle://book?action=open&asin=B0BNJ8KHYN&location=1257) ^ref-64366

---
Some developers query the database using other channels (such as Command and Query Responsibility Segregation (CQRS), — location: [1263](kindle://book?action=open&asin=B0BNJ8KHYN&location=1263) ^ref-46077

---
One mistake we often make with repository layers is to make one struct per database table. This should be avoided; instead, aim to make one struct per aggregate. — location: [1267](kindle://book?action=open&asin=B0BNJ8KHYN&location=1267) ^ref-19446

---
a repository layer can write to multiple tables. — location: [1273](kindle://book?action=open&asin=B0BNJ8KHYN&location=1273) ^ref-64549

---
We define this interface in the same package as our Booking factory and our service layer — location: [1279](kindle://book?action=open&asin=B0BNJ8KHYN&location=1279) ^ref-8156

---
In DDD, we use a few different types of services to help us organize our code. These are application services, domain services, and infrastructure services. — location: [1300](kindle://book?action=open&asin=B0BNJ8KHYN&location=1300) ^ref-16526

---
Domain services are stateless operations within a domain that complete a certain activity. — location: [1304](kindle://book?action=open&asin=B0BNJ8KHYN&location=1304) ^ref-55082

---
The code you are about to write performs a significant piece of business logic within one domain — location: [1308](kindle://book?action=open&asin=B0BNJ8KHYN&location=1308) ^ref-30909

---
You are taking the properties of two or more domain objects to calculate a value — location: [1310](kindle://book?action=open&asin=B0BNJ8KHYN&location=1310) ^ref-5810

---
Application services are used to compose other services and repositories. — location: [1341](kindle://book?action=open&asin=B0BNJ8KHYN&location=1341) ^ref-31749

---
They are responsible for managing transactional guarantees in place among various models. — location: [1342](kindle://book?action=open&asin=B0BNJ8KHYN&location=1342) ^ref-4589

---
They should not contain domain logic (this belongs in the domain service, as discussed in the previous section). — location: [1343](kindle://book?action=open&asin=B0BNJ8KHYN&location=1343) ^ref-64328

---
Application services are usually very thin. They are used only for coordination, and all the other logic should be pushed down into the layers underneath the application layer. Typically, we also address security concerns in this layer. — location: [1344](kindle://book?action=open&asin=B0BNJ8KHYN&location=1344) ^ref-45841

---
In this specific instance, it would have been fine for our domain service to do the persistence too (since we do not cross any domain boundaries). — location: [1362](kindle://book?action=open&asin=B0BNJ8KHYN&location=1362) ^ref-42030

---
One other use case for application services is to power a user interface (UI). — location: [1364](kindle://book?action=open&asin=B0BNJ8KHYN&location=1364) ^ref-17762

---
Accept payment (perhaps using Stripe or PayPal) Send email (perhaps using Amazon SES or Mailchimp) Track user behavior (perhaps using Mixpanel or Google Analytics) None of these functions are part of our primary domain, but we still want to include them in our application. To do this, we can use an infrastructure service. — location: [1371](kindle://book?action=open&asin=B0BNJ8KHYN&location=1371) ^ref-45291

---
This can then be added to your application service or domain service. — location: [1375](kindle://book?action=open&asin=B0BNJ8KHYN&location=1375) ^ref-55930

---
We call it a monolithic application if all the different components of the system are encapsulated into a single unit – for example, if the user interface, several domains, and infrastructure services are combined into a single deployable unit. The following figure illustrates this: — location: [1478](kindle://book?action=open&asin=B0BNJ8KHYN&location=1478) ^ref-16353

---
They are simple to develop. All code and concerns exist in a single place, — location: [1484](kindle://book?action=open&asin=B0BNJ8KHYN&location=1484) ^ref-25776

---
They are simple to deploy. There is only one deployable, and its requirements should be well understood. — location: [1486](kindle://book?action=open&asin=B0BNJ8KHYN&location=1486) ^ref-18603

---
They are simple to scale (to a point). — location: [1487](kindle://book?action=open&asin=B0BNJ8KHYN&location=1487) ^ref-27713

---
The startup time for the application can become multiple minutes. — location: [1490](kindle://book?action=open&asin=B0BNJ8KHYN&location=1490) ^ref-49043

---
Scaling the application starts to become difficult. — location: [1491](kindle://book?action=open&asin=B0BNJ8KHYN&location=1491) ^ref-27488

---
monoliths can only typically scale in one dimension. — location: [1492](kindle://book?action=open&asin=B0BNJ8KHYN&location=1492) ^ref-2228

---
Continuous deployment becomes slow. Even if you make a small code change to a specific part, you must deploy the entire application. — location: [1495](kindle://book?action=open&asin=B0BNJ8KHYN&location=1495) ^ref-30166

---
A long-term commitment to a specific technology stack is necessary. — location: [1497](kindle://book?action=open&asin=B0BNJ8KHYN&location=1497) ^ref-55583

---
Changes become difficult to make. — location: [1500](kindle://book?action=open&asin=B0BNJ8KHYN&location=1500) ^ref-12089

---
We spoke about what would be a good minimum viable product (MVP) for the new system that we will create. — location: [1527](kindle://book?action=open&asin=B0BNJ8KHYN&location=1527) ^ref-49600

---
The internal folder is a special folder in Golang. Anything within the internal directory cannot be imported by other projects. — location: [1548](kindle://book?action=open&asin=B0BNJ8KHYN&location=1548) ^ref-53611

---
Is it possible for me to treat this object as immutable? Does it measure, quantify, or describe a domain concept? Can it be compared to other objects of the same type just by its values? — location: [1594](kindle://book?action=open&asin=B0BNJ8KHYN&location=1594) ^ref-12914

---
it is better to treat something as a value object and then upgrade it to an entity later, as it’s a safer construct to deal with. — location: [1598](kindle://book?action=open&asin=B0BNJ8KHYN&location=1598) ^ref-34620

---
A purchase is a good fit for service because of the following: We are about to perform a significant piece of business logic within our domain We need to calculate some values We need to interact with the repository layer — location: [1714](kindle://book?action=open&asin=B0BNJ8KHYN&location=1714) ^ref-47734

---
Remember, we should always be trying to push down as much logic as possible into our domain objects: — location: [1720](kindle://book?action=open&asin=B0BNJ8KHYN&location=1720) ^ref-55018

---
We could meet with the payment team and agree on a contract for what CardService will look like (in Go, we call these contracts interfaces), and then we can continue with our implementations at separate paces. — location: [1783](kindle://book?action=open&asin=B0BNJ8KHYN&location=1783) ^ref-60759

---
The reason we do this is to decouple our purchase aggregate from the Mongo implementation. We should also decouple all the other domain models from the database models, — location: [1874](kindle://book?action=open&asin=B0BNJ8KHYN&location=1874) ^ref-11836

---
Like our Mongo repository, we are going to decouple ourselves from Stripe as much as possible, as it is not part of our domain, and it is a tool that the company may change its mind on in the future. — location: [1880](kindle://book?action=open&asin=B0BNJ8KHYN&location=1880) ^ref-57594

---
The service can be developed, deployed, and scaled independently; it should not impact the function of other services. — location: [2252](kindle://book?action=open&asin=B0BNJ8KHYN&location=2252) ^ref-1684

---
It does not share code with other services, and communication with other services happens over some form of RPC. — location: [2252](kindle://book?action=open&asin=B0BNJ8KHYN&location=2252) ^ref-41124

---
The service does not depend on other services being available to be successful. — location: [2254](kindle://book?action=open&asin=B0BNJ8KHYN&location=2254) ^ref-10588

---
Microservices enable teams to move fast. — location: [2261](kindle://book?action=open&asin=B0BNJ8KHYN&location=2261) ^ref-35620

---
Flexible scaling. — location: [2263](kindle://book?action=open&asin=B0BNJ8KHYN&location=2263) ^ref-31104

---
Easier deployments. — location: [2264](kindle://book?action=open&asin=B0BNJ8KHYN&location=2264) ^ref-16258

---
Freedom to explore different technologies. — location: [2267](kindle://book?action=open&asin=B0BNJ8KHYN&location=2267) ^ref-32573

---
More resilient. — location: [2268](kindle://book?action=open&asin=B0BNJ8KHYN&location=2268) ^ref-35797

---
Testing user journeys can be much harder, especially in event-driven systems. — location: [2277](kindle://book?action=open&asin=B0BNJ8KHYN&location=2277) ^ref-48127

---
Notice here how we have not coupled our interface to the partnership’s implementation at all. We have used domain language from our bounded context and defined what a reasonable, sensible interface — location: [2370](kindle://book?action=open&asin=B0BNJ8KHYN&location=2370) ^ref-51432

---
the adaptor pattern is useful for decoupling two different bounded contexts from each other, which helps separate concerns and ensure our systems can evolve independently and safely. — location: [2414](kindle://book?action=open&asin=B0BNJ8KHYN&location=2414) ^ref-17337

---
could use to do this is to generate an API using OpenAPI or gRPC, — location: [2475](kindle://book?action=open&asin=B0BNJ8KHYN&location=2475) ^ref-615

---
A distributed system is characterized as various computing components that are spread out over a network. — location: [2631](kindle://book?action=open&asin=B0BNJ8KHYN&location=2631) ^ref-14579

---
A distributed system usually has the following characteristics: — location: [2640](kindle://book?action=open&asin=B0BNJ8KHYN&location=2640) ^ref-58996

---
Scalable: The system can grow as workloads increase. — location: [2641](kindle://book?action=open&asin=B0BNJ8KHYN&location=2641) ^ref-5981

---
Fault-tolerant: If one piece of our system fails, it shouldn’t all — location: [2643](kindle://book?action=open&asin=B0BNJ8KHYN&location=2643) ^ref-32489

---
Transparent: Our system appears as a single unit to our end users; they do not need to worry about the underlying implementation. — location: [2647](kindle://book?action=open&asin=B0BNJ8KHYN&location=2647) ^ref-584

---
Concurrent: Multiple activities can happen at the same time within our system. — location: [2649](kindle://book?action=open&asin=B0BNJ8KHYN&location=2649) ^ref-42864

---
Heterogenous: This is a fancy word that means we can use a variety of servers, programming languages, and paradigms. — location: [2650](kindle://book?action=open&asin=B0BNJ8KHYN&location=2650) ^ref-59565

---
Replicated: Information is often replicated to enable fault tolerance. — location: [2653](kindle://book?action=open&asin=B0BNJ8KHYN&location=2653) ^ref-27261

---
CAP theorem. The CAP theorem states you must pick two of the following categories to make guarantees about, and the third you must accept will suffer. — location: [2657](kindle://book?action=open&asin=B0BNJ8KHYN&location=2657) ^ref-47467

---
Consistency: Every read receives the most up-to-date information or an error. — location: [2659](kindle://book?action=open&asin=B0BNJ8KHYN&location=2659) ^ref-60887

---
Availability: Every request receives a non-error response, but it may not receive the most up-to-date information. — location: [2660](kindle://book?action=open&asin=B0BNJ8KHYN&location=2660) ^ref-42402

---
Partition tolerance: The system continues to operate even if there are network issues happening (such as packets being dropped). — location: [2661](kindle://book?action=open&asin=B0BNJ8KHYN&location=2661) ^ref-9186

---
Canceling the operation and thus decreasing the availability but ensuring consistency — location: [2663](kindle://book?action=open&asin=B0BNJ8KHYN&location=2663) ^ref-12742

---
Proceeding with the operation and thus providing availability but risking inconsistency — location: [2664](kindle://book?action=open&asin=B0BNJ8KHYN&location=2664) ^ref-26334

---
You’ll often see CAP theorem trade-offs used for describing databases. — location: [2668](kindle://book?action=open&asin=B0BNJ8KHYN&location=2668) ^ref-61631

---
This means it delivers consistency and partition tolerance, but it does so at the expense of availability. — location: [2670](kindle://book?action=open&asin=B0BNJ8KHYN&location=2670) ^ref-34455

---
Mongo has a single primary node. This node must receive all write operations. Once persisted, these new writes are replicated to secondary nodes. — location: [2671](kindle://book?action=open&asin=B0BNJ8KHYN&location=2671) ^ref-65496

---
By default, clients read from the primary node to ensure they get the most recent information, but they can also read from a secondary node if configured to do so. — location: [2672](kindle://book?action=open&asin=B0BNJ8KHYN&location=2672) ^ref-4730

---
If the primary goes down, a secondary with the most recent data is promoted. — location: [2674](kindle://book?action=open&asin=B0BNJ8KHYN&location=2674) ^ref-11737

---
The database is unavailable at this time. — location: [2674](kindle://book?action=open&asin=B0BNJ8KHYN&location=2674) ^ref-54031

---
Once all the secondaries catch up, the database system becomes available again. — location: [2674](kindle://book?action=open&asin=B0BNJ8KHYN&location=2674) ^ref-49160

---
Alternatively, Cassandra is an AP database. Cassandra prioritizes availability and partition tolerance but sacrifices consistency. — location: [2678](kindle://book?action=open&asin=B0BNJ8KHYN&location=2678) ^ref-29872

---
Cassandra has no primary, and you can write to any of the nodes. Cassandra claims that it can survive the complete loss of a data center and has no single point of failure (SPOF) due to all the nodes being the same. — location: [2679](kindle://book?action=open&asin=B0BNJ8KHYN&location=2679) ^ref-25616

---
Those who know a little about CQRS might be surprised that one of the first mentions of it in a book about DDD is in the distributed system section. Let’s — location: [2696](kindle://book?action=open&asin=B0BNJ8KHYN&location=2696) ^ref-33562

---
CQRS is not necessary for DDD, but the sort of complex systems that benefit from DDD may also benefit from exploring CQRS; both are there to help you model and manage complexity. — location: [2709](kindle://book?action=open&asin=B0BNJ8KHYN&location=2709) ^ref-9852

---
follow a few simple rules while implementing CQRS. These are as follows: — location: [2712](kindle://book?action=open&asin=B0BNJ8KHYN&location=2712) ^ref-17619

---
Every method should be a command that performs an action or a query that answers a question. However, no method should do both. — location: [2712](kindle://book?action=open&asin=B0BNJ8KHYN&location=2712) ^ref-16790

---
Asking a question should not change the answer; queries should not mutate. — location: [2714](kindle://book?action=open&asin=B0BNJ8KHYN&location=2714) ^ref-21951

---
For object-oriented (OO) languages such as Java, these rules are extended to include the following: — location: [2715](kindle://book?action=open&asin=B0BNJ8KHYN&location=2715) ^ref-52548

---
If a method modifies the state of an object, it is a command. It should return void. — location: [2717](kindle://book?action=open&asin=B0BNJ8KHYN&location=2717) ^ref-57050

---
If a method returns a value and its query, it is answering a question. They should not modify the state of an object. — location: [2718](kindle://book?action=open&asin=B0BNJ8KHYN&location=2718) ^ref-20588

---
We can adapt these to Golang, as follows: — location: [2719](kindle://book?action=open&asin=B0BNJ8KHYN&location=2719) ^ref-40122

---
If a method modifies the state of the receiver struct or database, it is a command and should return an error or nil — location: [2720](kindle://book?action=open&asin=B0BNJ8KHYN&location=2720) ^ref-54551

---
If a method returns a value, it should not modify the database or its receiver struct — location: [2721](kindle://book?action=open&asin=B0BNJ8KHYN&location=2721) ^ref-25427

---
it can work fantastically well for event-based systems — location: [2729](kindle://book?action=open&asin=B0BNJ8KHYN&location=2729) ^ref-54678

---
Commands are a great way to model domain-event emission — location: [2730](kindle://book?action=open&asin=B0BNJ8KHYN&location=2730) ^ref-58245

---
EDA is a pattern in which our distributed system produces, detects, and responds to events. — location: [2732](kindle://book?action=open&asin=B0BNJ8KHYN&location=2732) ^ref-49854

---
An event is defined as a significant change in state. — location: [2733](kindle://book?action=open&asin=B0BNJ8KHYN&location=2733) ^ref-30239

---
Events are typically made up of two parts: an event header and an event body. — location: [2737](kindle://book?action=open&asin=B0BNJ8KHYN&location=2737) ^ref-36588

---
The event header will usually contain some meta-information about the message. For example, it might include a timestamp of when the message was emitted, the system that emitted it, and a unique identifier (UID) for that specific message. — location: [2738](kindle://book?action=open&asin=B0BNJ8KHYN&location=2738) ^ref-57167

---
The body usually contains information about the state that changed. — location: [2740](kindle://book?action=open&asin=B0BNJ8KHYN&location=2740) ^ref-52066

---
In the preceding example, we have used JSON format, but some other formats popular for defining message schemas are Protobuf, Apache Avro, and Cap’n Proto. — location: [2743](kindle://book?action=open&asin=B0BNJ8KHYN&location=2743) ^ref-9596

---
The message type we are interested in regarding DDD is domain events. For example, we might be interested in a message called user.loggedIn or purchase.failed. — location: [2746](kindle://book?action=open&asin=B0BNJ8KHYN&location=2746) ^ref-40001

---
These domain events might have significance in one specific bounded context but mean nothing to another. — location: [2749](kindle://book?action=open&asin=B0BNJ8KHYN&location=2749) ^ref-50422

---
there is no expectation that every system is interested in every domain event. — location: [2750](kindle://book?action=open&asin=B0BNJ8KHYN&location=2750) ^ref-63088

---
In this example, you can see how a long-running process starts with us initiating a long-running task that goes through a series of pipeline steps before it becomes useful at the end. — location: [2757](kindle://book?action=open&asin=B0BNJ8KHYN&location=2757) ^ref-19820

---
if I have a long-running process such as that defined previously, and someone changes their address mid-way through the process, how do we handle that? — location: [2764](kindle://book?action=open&asin=B0BNJ8KHYN&location=2764) ^ref-2408

---
consistency is equally (if not more so) important in a distributed system as it is in a monolithic architecture. However, it is near impossible to create distributed transactions and commit atomically. One approach to solve this is to split our work into two phases: — location: [2774](kindle://book?action=open&asin=B0BNJ8KHYN&location=2774) ^ref-45045

---
Preparation phase: We ask each of our sub-systems if it can promise to do the workload we want to complete. — location: [2776](kindle://book?action=open&asin=B0BNJ8KHYN&location=2776) ^ref-17940

---
Completion phase: Tell each sub-system to do the work it just promised to do. — location: [2777](kindle://book?action=open&asin=B0BNJ8KHYN&location=2777) ^ref-53059

---
2PC is a useful pattern to be aware of when building a domain-driven system. — location: [2784](kindle://book?action=open&asin=B0BNJ8KHYN&location=2784) ^ref-65407

---
The biggest disadvantage of the 2PC is the fact that it’s a blocking protocol. This means in the best case we lose some of the concurrency ability within our system, and in the worst case, no work can be completed at all until the lock is released — location: [2787](kindle://book?action=open&asin=B0BNJ8KHYN&location=2787) ^ref-16399

---
The saga pattern aims to allow us to achieve consistency within a distributed system without preventing concurrency. — location: [2792](kindle://book?action=open&asin=B0BNJ8KHYN&location=2792) ^ref-62832

---
The basic principle of the saga pattern is a simple one; for each action we take within our system, we also define a compensating action that we call in the event we need to roll back. — location: [2793](kindle://book?action=open&asin=B0BNJ8KHYN&location=2793) ^ref-20547

---
If all these steps successfully resolve or roll back, we should have a consistent system. — location: [2801](kindle://book?action=open&asin=B0BNJ8KHYN&location=2801) ^ref-28474

---
we can combine the saga pattern with an EDA (that we mentioned previously) and emit an event for compensating control. This means it can be retried by consumer services at their own pace and using their own patterns. — location: [2802](kindle://book?action=open&asin=B0BNJ8KHYN&location=2802) ^ref-53824

---
In the preceding code block, we declare an interface called Saga. Anything that has an Execute function that returns an error and a Rollback function that returns an error satisfies our Saga interface. — location: [2821](kindle://book?action=open&asin=B0BNJ8KHYN&location=2821) ^ref-38417

---
A shared file could technically satisfy the definition of a message bus (and that is kind of what Kafka is). — location: [2840](kindle://book?action=open&asin=B0BNJ8KHYN&location=2840) ^ref-47039

---
Kafka — location: [2847](kindle://book?action=open&asin=B0BNJ8KHYN&location=2847) ^ref-2815

---
Kafka can be scaled to achieve millions of requests per second and is popular at internet-scale companies such as Microsoft and Cloudflare due to its ability to scale and keep latency low, while also being fault-tolerant. — location: [2849](kindle://book?action=open&asin=B0BNJ8KHYN&location=2849) ^ref-39289

---
Firstly, we have a broker. This is responsible for storing messages sent in topics. — location: [2854](kindle://book?action=open&asin=B0BNJ8KHYN&location=2854) ^ref-52155

---
Topics can be split into many partitions. — location: [2855](kindle://book?action=open&asin=B0BNJ8KHYN&location=2855) ^ref-21616

---
Producers are services that connect to Kafka to send messages. — location: [2855](kindle://book?action=open&asin=B0BNJ8KHYN&location=2855) ^ref-63801

---
Consumers subscribe to topics and partitions to read messages. — location: [2856](kindle://book?action=open&asin=B0BNJ8KHYN&location=2856) ^ref-28082

---
Services can be both consumers and producers. — location: [2859](kindle://book?action=open&asin=B0BNJ8KHYN&location=2859) ^ref-39153

---
RabbitMQ — location: [2864](kindle://book?action=open&asin=B0BNJ8KHYN&location=2864) ^ref-50773

---
It is easy to get started with and conceptually is simple. — location: [2865](kindle://book?action=open&asin=B0BNJ8KHYN&location=2865) ^ref-58224

---
Once a message has been read from a queue and acknowledged by a producer application, it is consumed and will never be received again. — location: [2866](kindle://book?action=open&asin=B0BNJ8KHYN&location=2866) ^ref-29056

---
publisher sends messages to an exchange. Based on the routing key, it is sent to a specific queue where is it picked up by a consumer application to process. — location: [2874](kindle://book?action=open&asin=B0BNJ8KHYN&location=2874) ^ref-61776

---
The disadvantages of RabbitMQ are mostly that it doesn’t scale quite as well or as easily as Kafka. It also only offers a subset of the features that Kafka does. — location: [2876](kindle://book?action=open&asin=B0BNJ8KHYN&location=2876) ^ref-15187

---
NATS — location: [2879](kindle://book?action=open&asin=B0BNJ8KHYN&location=2879) ^ref-15031

---
Neural Autonomic Transport System (NATS) is an open source streaming system written in Golang. — location: [2880](kindle://book?action=open&asin=B0BNJ8KHYN&location=2880) ^ref-21401

---
One nice feature of NATS is the ability to wildcard match on topics such as those shown here: — location: [2884](kindle://book?action=open&asin=B0BNJ8KHYN&location=2884) ^ref-24325

---
NATS guarantees at-most-once delivery, which is to say your message might never be delivered at all. — location: [2888](kindle://book?action=open&asin=B0BNJ8KHYN&location=2888) ^ref-29651

---
TDD stands for test-driven development. It is a process in which you write tests for business requirements before your software is fully developed. — location: [2921](kindle://book?action=open&asin=B0BNJ8KHYN&location=2921) ^ref-9341

---
As you write code, you repeatedly update your test cases until you are satisfied the code satisfies the business requirements. — location: [2923](kindle://book?action=open&asin=B0BNJ8KHYN&location=2923) ^ref-23170

---
The goal is to write “just enough” code to pass the tests and no more. — location: [2924](kindle://book?action=open&asin=B0BNJ8KHYN&location=2924) ^ref-28301

---
Add a test: Before we write any code, we write the test case. — location: [2928](kindle://book?action=open&asin=B0BNJ8KHYN&location=2928) ^ref-7284

---
Run the test we just wrote. It should fail (and we should expect it to): — location: [2935](kindle://book?action=open&asin=B0BNJ8KHYN&location=2935) ^ref-2730

---
Write as little code as possible to pass the test: — location: [2938](kindle://book?action=open&asin=B0BNJ8KHYN&location=2938) ^ref-29796

---
The goal is to get that test case passing by any means necessary while solving for the business invariant. — location: [2939](kindle://book?action=open&asin=B0BNJ8KHYN&location=2939) ^ref-39769

---
Rerun the tests – the new one and all the previous ones should now pass: — location: [2940](kindle://book?action=open&asin=B0BNJ8KHYN&location=2940) ^ref-29680

---
Refactor: — location: [2943](kindle://book?action=open&asin=B0BNJ8KHYN&location=2943) ^ref-30355

---

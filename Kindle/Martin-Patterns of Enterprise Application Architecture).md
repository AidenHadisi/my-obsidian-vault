---
kindle-sync:
  bookId: '54390'
  title: >-
    Patterns of Enterprise Application Architecture (Addison-Wesley Signature
    Series (Fowler))
  author: Fowler Martin
  asin: B008OHVDFM
  lastAnnotatedDate: '2024-09-17'
  bookImageUrl: 'https://m.media-amazon.com/images/I/81VEh8RJOlL._SY160.jpg'
  highlightsCount: 520
---
# Patterns of Enterprise Application Architecture)
## Metadata
* Author: [Fowler Martin](https://www.amazon.comundefined)
* ASIN: B008OHVDFM
* Reference: https://www.amazon.com/dp/B008OHVDFM
* [Kindle link](kindle://book?action=open&asin=B008OHVDFM)

## Highlights
Layering is one of the most common techniques that software designers use to break apart a complicated software system. — location: [665](kindle://book?action=open&asin=B008OHVDFM&location=665) ^ref-18897

---
In this scheme the higher layer uses various services defined by the lower layer, but the lower layer is unaware of the higher layer. — location: [669](kindle://book?action=open&asin=B008OHVDFM&location=669) ^ref-60652

---
Furthermore, each layer usually hides its lower layers from the layers above, so layer 4 uses the services of layer 3, which uses the services of layer 2, but layer 4 is unaware of layer 2. — location: [670](kindle://book?action=open&asin=B008OHVDFM&location=670) ^ref-40833

---
Breaking down a system into layers has a number of important benefits. — location: [672](kindle://book?action=open&asin=B008OHVDFM&location=672) ^ref-41500

---
You can understand a single layer as a coherent whole without knowing much about the other layers. — location: [673](kindle://book?action=open&asin=B008OHVDFM&location=673) ^ref-57233

---
You can substitute layers with alternative implementations of the same basic services. — location: [674](kindle://book?action=open&asin=B008OHVDFM&location=674) ^ref-30975

---
You minimize dependencies between layers. — location: [676](kindle://book?action=open&asin=B008OHVDFM&location=676) ^ref-6109

---
Layers make good places for standardization. TCP and IP are standards because they define how their layers should operate. — location: [678](kindle://book?action=open&asin=B008OHVDFM&location=678) ^ref-28787

---
Once you have a layer built, you can use it for many higher-level services. — location: [679](kindle://book?action=open&asin=B008OHVDFM&location=679) ^ref-20526

---
but there are downsides. — location: [681](kindle://book?action=open&asin=B008OHVDFM&location=681) ^ref-44546

---
Layers encapsulate some, but not all, things well. As a result you sometimes get cascading changes. The classic example of this in a layered enterprise application is adding a field that needs to display on the UI, must be in the database, and thus must be added to every layer in between. — location: [681](kindle://book?action=open&asin=B008OHVDFM&location=681) ^ref-21180

---
Extra layers can harm performance. At every layer things typically need to be transformed from one representation to another. — location: [684](kindle://book?action=open&asin=B008OHVDFM&location=684) ^ref-51224

---
But the hardest part of a layered architecture is deciding what layers to have and what the responsibility of each layer should be. — location: [686](kindle://book?action=open&asin=B008OHVDFM&location=686) ^ref-52554

---
The notion of layers became more apparent in the ’90s with the rise of client–server systems. — location: [690](kindle://book?action=open&asin=B008OHVDFM&location=690) ^ref-57458

---
The object community had an answer to the problem of domain logic: Move to a three-layer system. In this approach you have a presentation layer for your UI, a domain layer for your domain logic, and a data source. — location: [702](kindle://book?action=open&asin=B008OHVDFM&location=702) ^ref-40275

---
browser. However, if all your business logic was buried in a rich client, then all your business logic needed to be redone to have a Web interface. — location: [708](kindle://book?action=open&asin=B008OHVDFM&location=708) ^ref-42037

---
Table 1.1. Three Principal Layers — location: [719](kindle://book?action=open&asin=B008OHVDFM&location=719) ^ref-16827

---
Presentation logic is about how to handle the interaction between the user and the software. — location: [721](kindle://book?action=open&asin=B008OHVDFM&location=721) ^ref-2168

---
The primary responsibilities of the presentation layer are to display information to the user and to interpret commands from the user into actions upon the domain and data source. — location: [723](kindle://book?action=open&asin=B008OHVDFM&location=723) ^ref-3172

---
Data source logic is about communicating with other systems that carry out tasks on behalf of the application. — location: [725](kindle://book?action=open&asin=B008OHVDFM&location=725) ^ref-12612

---
The remaining piece is the domain logic, also referred to as business logic. This is the work that this application needs to do for the domain you’re working with. It involves calculations based on inputs and stored data, validation of any data that comes in from the presentation, and figuring out exactly what data source logic to dispatch, depending on commands received from the presentation. — location: [727](kindle://book?action=open&asin=B008OHVDFM&location=727) ^ref-34783

---
Sometimes the layers are arranged so that the domain layer completely hides the data source from the presentation. More often, however, the presentation accesses the data store directly. While this is less pure, it tends to work better in practice. The presentation may interpret a command from the user, use the data source to pull the relevant data out of the database, and then let the domain logic manipulate that data before presenting it on the glass. — location: [730](kindle://book?action=open&asin=B008OHVDFM&location=730) ^ref-20276

---
At this point it becomes apparent that there is a lot of similarity between the presentation and data source layers in that they both are about connection to the outside world. — location: [740](kindle://book?action=open&asin=B008OHVDFM&location=740) ^ref-55645

---
Presentation is an external interface for a service your system offers to someone else, whether it be a complex human or a simple remote program. Data source is the interface to things that are providing a service to you. — location: [745](kindle://book?action=open&asin=B008OHVDFM&location=745) ^ref-30875

---
My general advice is to choose the most appropriate form of separation for your problem but make sure you do some kind of separation—at least at the subroutine level. — location: [752](kindle://book?action=open&asin=B008OHVDFM&location=752) ^ref-44397

---
The domain and data source should never be dependent on the presentation. — location: [754](kindle://book?action=open&asin=B008OHVDFM&location=754) ^ref-15911

---
That is, there should be no subroutine call from the domain or data source code into the presentation code. — location: [754](kindle://book?action=open&asin=B008OHVDFM&location=754) ^ref-8011

---
The relationship between the domain and the data source is more complex and depends upon the architectural patterns used for the data source. — location: [756](kindle://book?action=open&asin=B008OHVDFM&location=756) ^ref-63127

---
An informal test I like is to imagine adding a radically different layer to an application, such as a command-line interface to a Web application. If there’s any functionality you have to duplicate in order to do this, that’s a sign of where domain logic has leaked into the presentation. Similarly, do you have to duplicate logic to replace a relational database with an XML file? — location: [759](kindle://book?action=open&asin=B008OHVDFM&location=759) ^ref-46125

---
The trouble is that that’s putting domain logic into the presentation. To properly separate the layers you need a method in the domain layer to indicate if a product has improving sales. — location: [764](kindle://book?action=open&asin=B008OHVDFM&location=764) ^ref-53670

---
The general argument in favor of running on a client turns on responsiveness or disconnected operation. Any logic that runs on the server needs a server roundtrip to respond to anything the user does. If the user wants to fiddle with things and see immediate feedback, that roundtrip gets in the way. — location: [777](kindle://book?action=open&asin=B008OHVDFM&location=777) ^ref-49436

---
The data source pretty much always runs only on servers. — location: [783](kindle://book?action=open&asin=B008OHVDFM&location=783) ^ref-59430

---
The decision of where to run the presentation depends mostly on what kind of user interface you want. Running a rich client pretty much means running the presentation on the client. — location: [785](kindle://book?action=open&asin=B008OHVDFM&location=785) ^ref-32636

---
Running a Web interface pretty much means running on the server. — location: [787](kindle://book?action=open&asin=B008OHVDFM&location=787) ^ref-3829

---
This leaves us with the domain logic. You can run business logic all on the server or all on the client, or you can split it. Again, all on the server is the best choice for ease of maintenance. The demand to move it to the client is for either responsiveness or disconnected use. — location: [798](kindle://book?action=open&asin=B008OHVDFM&location=798) ^ref-38437

---
If you have to run some logic on the client, you can consider running all of it there—at least that way it’s all in one place. — location: [800](kindle://book?action=open&asin=B008OHVDFM&location=800) ^ref-56707

---
The simplest approach to storing domain logic is the Transaction Script (110). A Transaction Script (110) is essentially a procedure that takes the input from the presentation, processes it with validations and calculations, stores data in the database, and invokes any operations from other systems. It then replies with more data to the presentation, perhaps doing more calculation to help organize and format the reply. — location: [820](kindle://book?action=open&asin=B008OHVDFM&location=820) ^ref-24469

---
Hence, we can think of this pattern as being a script for an action, or business transaction. — location: [824](kindle://book?action=open&asin=B008OHVDFM&location=824) ^ref-59319

---
the driving force is still that of a procedure for each action, so a retailing system might have Transaction Scripts (110) for checkout, for adding something to the shopping cart, for displaying delivery status, and so on. — location: [826](kindle://book?action=open&asin=B008OHVDFM&location=826) ^ref-10932

---
It’s a simple procedural model that most developers understand. — location: [829](kindle://book?action=open&asin=B008OHVDFM&location=829) ^ref-39844

---
works well with a simple data source layer using Row Data Gateway (152) or Table Data Gateway — location: [830](kindle://book?action=open&asin=B008OHVDFM&location=830) ^ref-55138

---
It’s obvious how to set the transaction boundaries: Start with opening a transaction and end with closing it. — location: [832](kindle://book?action=open&asin=B008OHVDFM&location=832) ^ref-57447

---
Often there will be duplicated code as several transactions need to do similar things. — location: [835](kindle://book?action=open&asin=B008OHVDFM&location=835) ^ref-37130

---
The resulting application can end up being quite a tangled web of routines without a clear structure. — location: [836](kindle://book?action=open&asin=B008OHVDFM&location=836) ^ref-53689

---
With a Domain Model (116) we build a model of our domain which, at least on a first approximation, is organized primarily around the nouns in the domain. — location: [838](kindle://book?action=open&asin=B008OHVDFM&location=838) ^ref-15011

---
The logic for handling validations and calculations would be placed into this domain model, so shipment object might contain the logic to calculate the shipping charge for a delivery. — location: [840](kindle://book?action=open&asin=B008OHVDFM&location=840) ^ref-26080

---
Rather than one routine having all the logic for a user action, each object takes a part of the logic that’s relevant to it. — location: [845](kindle://book?action=open&asin=B008OHVDFM&location=845) ^ref-31335

---
In contrast, Figure 2.2 shows multiple objects, each forwarding part of the behavior to another until a strategy object creates the results. — location: [860](kindle://book?action=open&asin=B008OHVDFM&location=860) ^ref-34466

---
As we get more and more algorithms for calculating revenue recognition, we can add these by adding new recognition strategy objects. With Transaction Script (110) we’re adding more conditions to the conditional logic of the script. — location: [863](kindle://book?action=open&asin=B008OHVDFM&location=863) ^ref-35729

---
The richer your Domain Model (116), the more complex your mapping to a relational database — location: [872](kindle://book?action=open&asin=B008OHVDFM&location=872) ^ref-28758

---
There’s a third choice for structuring domain logic, Table Module — location: [876](kindle://book?action=open&asin=B008OHVDFM&location=876) ^ref-39927

---
The vital difference is that a Domain Model (116) has one instance of contract for each contract in the database whereas a Table Module (125) has only one instance. — location: [878](kindle://book?action=open&asin=B008OHVDFM&location=878) ^ref-16280

---
A Table Module (125) is in many ways a middle ground between a Transaction Script (110) and a Domain Model — location: [888](kindle://book?action=open&asin=B008OHVDFM&location=888) ^ref-28525

---
The biggest advantage of a Table Module (125) is how it fits into the rest of the architecture. — location: [893](kindle://book?action=open&asin=B008OHVDFM&location=893) ^ref-63868

---
With simple domain logic the Domain Model (116) is less attractive because the cost of understanding it and the complexity of the data source add a lot of effort to developing it that won’t be paid back. — location: [902](kindle://book?action=open&asin=B008OHVDFM&location=902) ^ref-22473

---
The attractiveness of a Table Module (125) depends very much on the support for a common Record Set (508) structure in your environment. — location: [914](kindle://book?action=open&asin=B008OHVDFM&location=914) ^ref-18115

---
However, if there’s no special tooling for Record Sets (508), I wouldn’t bother with Table Module — location: [919](kindle://book?action=open&asin=B008OHVDFM&location=919) ^ref-17183

---
A common approach in handling domain logic is to split the domain layer in two. A Service Layer (133) is placed over an underlying Domain Model (116) or Table Module — location: [929](kindle://book?action=open&asin=B008OHVDFM&location=929) ^ref-15901

---
The presentation logic interacts with the domain purely through the Service Layer (133), which acts as an API for the application. — location: [934](kindle://book?action=open&asin=B008OHVDFM&location=934) ^ref-25414

---
the Service Layer (133) is also a good spot to place such things as transaction control and security. — location: [936](kindle://book?action=open&asin=B008OHVDFM&location=936) ^ref-31314

---
When you see a Service Layer (133), a key decision is how much behavior to put in it. The minimal case is to make the Service Layer (133) a facade so that all of the real behavior is in underlying objects and all the Service Layer (133) does is forward calls on the facade to lower-level objects. — location: [939](kindle://book?action=open&asin=B008OHVDFM&location=939) ^ref-24637

---
At the other extreme, most business logic is placed in Transaction Scripts (110) inside the Service Layer (133). The underlying domain objects are very simple; if it’s a Domain Model (116) it will be one-to-one with the database and you can thus use a simpler data source layer such as Active Record (160). — location: [944](kindle://book?action=open&asin=B008OHVDFM&location=944) ^ref-6665

---
Midway between these alternatives is a more even mix of behavior: the controller-entity style. — location: [948](kindle://book?action=open&asin=B008OHVDFM&location=948) ^ref-5468

---
al.]. The point here is to have logic that’s particular to a single transaction or use case placed in Transaction Scripts (110), which are commonly referred to as controllers or services. — location: [950](kindle://book?action=open&asin=B008OHVDFM&location=950) ^ref-35709

---
The use case controllers, like any Transaction Script (110), tend to encourage duplicate code. — location: [955](kindle://book?action=open&asin=B008OHVDFM&location=955) ^ref-16848

---
Then it makes sense to move duplicated behavior to the Row Data Gateways (152), which will turn them into a simple Domain Model (116) using Active Record (160). — location: [959](kindle://book?action=open&asin=B008OHVDFM&location=959) ^ref-8059

---
My preference is thus to have the thinnest Service Layer (133) you can, if you even need one. — location: [965](kindle://book?action=open&asin=B008OHVDFM&location=965) ^ref-57521

---
The role of the data source layer is to communicate with the various pieces of infrastructure that an application needs to do its job. — location: [971](kindle://book?action=open&asin=B008OHVDFM&location=971) ^ref-23965

---
For these reasons, it’s wise to separate SQL access from the domain logic and place it in separate classes. — location: [983](kindle://book?action=open&asin=B008OHVDFM&location=983) ^ref-38852

---
A good way of organizing these classes is to base them on the table structure of the database so that you have one class per database table. These classes then form a Gateway (466) to the table. — location: [984](kindle://book?action=open&asin=B008OHVDFM&location=984) ^ref-65348

---
There are two main ways in which you can use a Gateway (466). The most obvious is to have an instance of it for each row that’s returned by a query (Figure 3.1). This Row Data Gateway (152) is an approach that naturally fits an object-oriented way of thinking about the data. — location: [987](kindle://book?action=open&asin=B008OHVDFM&location=987) ^ref-46146

---
A Row Data Gateway (152) has one instance per row returned by a query. — location: [991](kindle://book?action=open&asin=B008OHVDFM&location=991) ^ref-57697

---
If you use a Record Set (508), you only need a single class for each table in the database. — location: [996](kindle://book?action=open&asin=B008OHVDFM&location=996) ^ref-26669

---
Even for simple applications I tend to use one of the gateway patterns. — location: [1001](kindle://book?action=open&asin=B008OHVDFM&location=1001) ^ref-43341

---
The fact that Table Data Gateway (144) fits very nicely with Record Set (508) makes it the obvious choice if you are using Table Module (125). — location: [1002](kindle://book?action=open&asin=B008OHVDFM&location=1002) ^ref-20643

---
If you’re using Domain Model (116), some further options come into play. Certainly you can use a Row Data Gateway (152) or a Table Data Gateway (144) with a Domain Model (116). For my taste, however, that can be either too much indirection or not enough. — location: [1009](kindle://book?action=open&asin=B008OHVDFM&location=1009) ^ref-50525

---
In simple applications the Domain Model (116) is an uncomplicated structure that actually corresponds pretty closely to the database structure, with one domain class per database table. Such domain objects often have only moderately complex business logic. In this case it makes sense to have each domain object be responsible for loading and saving from the database, which is Active Record (160) — location: [1012](kindle://book?action=open&asin=B008OHVDFM&location=1012) ^ref-62601

---
The one-to-one match of domain classes to tables starts to fail as you factor domain logic into smaller classes. Relational databases don’t handle inheritance, so it becomes difficult to use strategies [Gang of Four] and other neat OO patterns. As the domain logic gets feisty, you want to be able to test it without having to talk to the database all the time. — location: [1024](kindle://book?action=open&asin=B008OHVDFM&location=1024) ^ref-19587

---
In this case the Gateway (466) can solve some problems, but it still leaves you with the Domain Model (116) coupled to the schema of the database. — location: [1028](kindle://book?action=open&asin=B008OHVDFM&location=1028) ^ref-31478

---
A better route is to isolate the Domain Model (116) from the database completely, by making your indirection layer entirely responsible for the mapping between domain objects and database tables. — location: [1032](kindle://book?action=open&asin=B008OHVDFM&location=1032) ^ref-4269

---
If the domain logic is simple and you have a close correspondence between classes and tables, Active Record (160) is the simple way to go. If you have something more complicated, Data Mapper (165) is what you need. — location: [1040](kindle://book?action=open&asin=B008OHVDFM&location=1040) ^ref-37797

---
Updating obviously is more complicated with views and queries, as you can’t always update a view directly but instead have to manipulate the tables that underlie it. In this case encapsulating the view/query with an appropriate pattern is a very good way to implement that update logic in one place, which makes using the views both simpler and more reliable. — location: [1051](kindle://book?action=open&asin=B008OHVDFM&location=1051) ^ref-38076

---
With an OO database you don’t have to worry about mapping. You work with a large structure of interconnected objects, and the database figures out when to move objects on or off disks. — location: [1060](kindle://book?action=open&asin=B008OHVDFM&location=1060) ^ref-16729

---
Even if you can’t use an OO database, you should seriously consider buying an O/R mapping tool if you have a Domain Model (116). — location: [1068](kindle://book?action=open&asin=B008OHVDFM&location=1068) ^ref-58622

---
When people talk about O/R mapping, they usually focus on the structural aspects—how you relate tables to objects. However, I’ve found that the hardest part of the exercise is its architectural and behavioral aspects. — location: [1079](kindle://book?action=open&asin=B008OHVDFM&location=1079) ^ref-51474

---
That behavioral problem is how to get the various objects to load and save themselves to the database. — location: [1081](kindle://book?action=open&asin=B008OHVDFM&location=1081) ^ref-6065

---
If you load a bunch of objects into memory and modify them, you have to keep track of which ones you’ve modified and make sure to write all of them back out to the database. — location: [1084](kindle://book?action=open&asin=B008OHVDFM&location=1084) ^ref-59868

---
If you read some objects, it’s important to ensure that the reading is isolated so that no other process changes any of the objects you’ve read while you’re working on them. Otherwise, you could have inconsistent and invalid data in your objects. — location: [1088](kindle://book?action=open&asin=B008OHVDFM&location=1088) ^ref-41696

---
(184). A Unit of Work (184) keeps track of all objects read from the database, together with all objects modified in any way. It also handles how updates are made to the database. — location: [1092](kindle://book?action=open&asin=B008OHVDFM&location=1092) ^ref-39485

---
A good way of thinking about Unit of Work (184) is as an object that acts as the controller of the database mapping. — location: [1097](kindle://book?action=open&asin=B008OHVDFM&location=1097) ^ref-32997

---
The Unit of Work (184) results from factoring the database mapping controller behavior into its own object. — location: [1099](kindle://book?action=open&asin=B008OHVDFM&location=1099) ^ref-49450

---
As you load objects, you have to be wary about loading the same one twice. If you do that, you’ll have two in-memory objects that correspond to a single database row. Update them both, and everything gets very confusing. — location: [1101](kindle://book?action=open&asin=B008OHVDFM&location=1101) ^ref-32713

---
(195). Each time you read in some data, you check the Identity Map (195) first to make sure that you don’t already have it. If the data is already loaded, you can return a second reference to it. — location: [1103](kindle://book?action=open&asin=B008OHVDFM&location=1103) ^ref-50462

---
As a benefit you may also be able to avoid a database call since the Identity Map (195) also doubles as a cache for the database. Don’t forget, however, that the primary purpose of an Identity Map (195) is to maintain correct identities, not to boost performance. — location: [1105](kindle://book?action=open&asin=B008OHVDFM&location=1105) ^ref-17132

---
If you’re using a Domain Model (116), you’ll usually arrange things so that linked objects are loaded together in such a way that a read for an order object loads its associated customer object. — location: [1108](kindle://book?action=open&asin=B008OHVDFM&location=1108) ^ref-1116

---
on. Lazy Load (200) relies on having a placeholder for a reference to an object. — location: [1112](kindle://book?action=open&asin=B008OHVDFM&location=1112) ^ref-41369

---
If your database interaction classes are table based—that is, you have one instance of the class per table in the database—then you can combine the finder methods with the inserts and updates. If your interaction classes are row based—that is, you have one interaction class per row in the database—this doesn’t work. — location: [1119](kindle://book?action=open&asin=B008OHVDFM&location=1119) ^ref-15644

---
With row-based classes you can make the find operations static, but doing so will stop you from making the database operations substitutable. — location: [1122](kindle://book?action=open&asin=B008OHVDFM&location=1122) ^ref-5568

---
To avoid this problem the best approach is to have separate finder objects. Each finder class has many methods that encapsulate a SQL query. — location: [1124](kindle://book?action=open&asin=B008OHVDFM&location=1124) ^ref-44694

---
Try to pull back multiple rows at once. In particular, never do repeated queries on the same table to get multiple rows. It’s almost always better to pull back too much data than too little — location: [1129](kindle://book?action=open&asin=B008OHVDFM&location=1129) ^ref-3846

---
It’s usually better to use one query that brings back unnecessary rows than to issue 50 individual queries. — location: [1133](kindle://book?action=open&asin=B008OHVDFM&location=1133) ^ref-39812

---
However, if you’re using joins, bear in mind that databases are optimized to handle up to three or four joins per query. Beyond that, performance suffers, — location: [1137](kindle://book?action=open&asin=B008OHVDFM&location=1137) ^ref-15916

---
aren’t usually relevant for Table Data Gateway (144), but you may use a few of them if you use Row Data Gateway (152) or Active Record (160). — location: [1146](kindle://book?action=open&asin=B008OHVDFM&location=1146) ^ref-42881

---
probably need to use all of them for Data Mapper — location: [1148](kindle://book?action=open&asin=B008OHVDFM&location=1148) ^ref-31610

---
The way to handle the representation problem is to keep the relational identity of each object as an Identity Field (216) in the object, and to look up these values to map back and forth between the object references and the relational keys. — location: [1156](kindle://book?action=open&asin=B008OHVDFM&location=1156) ^ref-56344

---
to wire up the appropriate inter-object reference. If you don’t have the key in the Identity Map (195), you need to either go to the database to get it or use a Lazy Load (200). — location: [1161](kindle://book?action=open&asin=B008OHVDFM&location=1161) ^ref-55802

---
If an object has a collection, you need to issue another query to find all the rows that link to the ID of the source object (or you can now avoid the query with Lazy Load (200)). — location: [1168](kindle://book?action=open&asin=B008OHVDFM&location=1168) ^ref-61943

---
If the collection objects aren’t used outside the scope of the collection’s owner, you can use Dependent Mapping (262) to simplify the mapping. — location: [1173](kindle://book?action=open&asin=B008OHVDFM&location=1173) ^ref-47191

---
An example is a person having many skills and each skill knowing the people who use it. — location: [1177](kindle://book?action=open&asin=B008OHVDFM&location=1177) ^ref-25278

---
it’s worth considering using unordered sets for storing collections. Another option is to decide on a sort order whenever you do a collection query, although that can be quite expensive. — location: [1184](kindle://book?action=open&asin=B008OHVDFM&location=1184) ^ref-1345

---
Small Value Objects (486), such as date ranges and money objects clearly shouldn’t be represented as their own table in the database. Instead, take all the fields of the Value Object (486) and embed them into the linked object as an Embedded Value (268). — location: [1191](kindle://book?action=open&asin=B008OHVDFM&location=1191) ^ref-46721

---
Writing them out is also easy—just dereference the object and spit out its fields into the owning table. — location: [1196](kindle://book?action=open&asin=B008OHVDFM&location=1196) ^ref-58704

---
You can do this kind of thing on a larger scale by taking a whole cluster of objects and saving them as a single column in a table as a Serialized LOB (272). — location: [1197](kindle://book?action=open&asin=B008OHVDFM&location=1197) ^ref-38888

---
Serializing a clump of objects as an XML document is an obvious route to take for a hierarchic object structure. — location: [1199](kindle://book?action=open&asin=B008OHVDFM&location=1199) ^ref-48247

---
Usually a Serialized LOB (272) is best for a relatively isolated group of objects that make part of an application. — location: [1206](kindle://book?action=open&asin=B008OHVDFM&location=1206) ^ref-30062

---
For any inheritance structure there are basically three options. You can have one table for all the classes in the hierarchy: Single Table Inheritance (278) (see Figure 3.8); one table for each concrete class: Concrete Table Inheritance (293) (see Figure 3.9); or one table per class in the hierarchy: Class Table Inheritance (285) (see Figure 3.10). — location: [1211](kindle://book?action=open&asin=B008OHVDFM&location=1211) ^ref-54927

---
The three options aren’t mutually exclusive, and in one hierarchy you can mix patterns. — location: [1232](kindle://book?action=open&asin=B008OHVDFM&location=1232) ^ref-57668

---
My first choice tends to be Single Table Inheritance (278), as it’s easy to do and is resilient to many refactorings. I tend to use the other two as needed to help solve the inevitable issues with irrelevant and wasted columns. — location: [1236](kindle://book?action=open&asin=B008OHVDFM&location=1236) ^ref-31433

---
Single Table Inheritance (278) puts all superclasses and interfaces into the one big table, Class Table Inheritance (285) makes a separate table for each interface and superclass, and Concrete Table Inheritance (293) includes all interfaces and superclasses in each concrete table. — location: [1242](kindle://book?action=open&asin=B008OHVDFM&location=1242) ^ref-4887

---
The simplest case is where you’re doing the schema yourself and have little to moderate complexity in your domain logic, resulting in a Transaction Script (110) or Table Module (125) design. — location: [1249](kindle://book?action=open&asin=B008OHVDFM&location=1249) ^ref-14888

---
In this case you can design the tables around the data using classic database design techniques. Use a Row Data Gateway (152) or Table Data Gateway (144) to pull the SQL away from the domain logic. — location: [1251](kindle://book?action=open&asin=B008OHVDFM&location=1251) ^ref-56445

---
Data Mapper (165) gives you the most flexibility here, but it’s more complex. If a database design isomorphic to the Domain Model (116) makes sense, you might consider an Active Record (160) instead. — location: [1257](kindle://book?action=open&asin=B008OHVDFM&location=1257) ^ref-61784

---
you should think about the Domain Model (116) first, but integrate each piece of Domain Model (116) in the database as you go. — location: [1264](kindle://book?action=open&asin=B008OHVDFM&location=1264) ^ref-3461

---
With simple domain logic you build Row Data Gateway (152) or Table Data Gateway (144) classes that mimic the database, and layer domain logic on top of that. — location: [1266](kindle://book?action=open&asin=B008OHVDFM&location=1266) ^ref-31238

---
The simplest option is to have multiple mapping layers, one for each data source. However, if data is very similar this can lead to a lot of duplication. — location: [1276](kindle://book?action=open&asin=B008OHVDFM&location=1276) ^ref-60582

---
Metadata Mapping (306) is based on boiling down the mapping into a metadata file that details how columns in the database map to fields in objects. The point of this is that once you have the metadata you can avoid the repetitive code by using either code generation or reflective programming. — location: [1287](kindle://book?action=open&asin=B008OHVDFM&location=1287) ^ref-50056

---
<field name = customer targetClass = "Customer", dbColumn = "custID", targetTable = "customers" lowerBound = "1" upperBound = "1" setter = "loadCustomer"/> — location: [1290](kindle://book?action=open&asin=B008OHVDFM&location=1290) ^ref-55587

---
From that you can define the read and write code, automatically generate ad hoc joins, do all of the SQL, enforce the multiplicity of the relationship, and even do fancy things like computing write orders under the presence of referential integrity. — location: [1292](kindle://book?action=open&asin=B008OHVDFM&location=1292) ^ref-21946

---
When you use Metadata Mapping (306) you have the necessary foundation to build queries in terms of in-memory objects. A Query Object (316) allows you to build your queries in terms of in-memory objects and data in such a way that developers don’t need to know either SQL or the details of the relational schema. The Query Object (316) can then use the Metadata Mapping (306) to translate expressions based on object fields into the appropriate SQL. — location: [1294](kindle://book?action=open&asin=B008OHVDFM&location=1294) ^ref-53429

---
Take this far enough and you can form a Repository (322) that largely hides the database from view. Any queries to the database can be made as Query Objects (316) against a Repository (322), and developers can’t tell whether the objects were retrieved from memory or from the database. — location: [1299](kindle://book?action=open&asin=B008OHVDFM&location=1299) ^ref-48400

---
In many environments it’s expensive to create a connection, which makes it worthwhile to create a connection pool. In this situation developers request a connection from the pool and release it when they’re done, instead of creating and closing the connection. — location: [1314](kindle://book?action=open&asin=B008OHVDFM&location=1314) ^ref-16681

---
A Unit of Work (184) makes a natural fit to manage both the transaction and the connection. — location: [1345](kindle://book?action=open&asin=B008OHVDFM&location=1345) ^ref-20517

---
Using select * can have serious problems in some database drivers, which break if a new column is added or a column is reordered. — location: [1355](kindle://book?action=open&asin=B008OHVDFM&location=1355) ^ref-52369

---
Consequently, if you’re using Table Data Gateway (144), you should use column name indices as the result set is used by every piece of code that runs a find operation on the gateway. — location: [1361](kindle://book?action=open&asin=B008OHVDFM&location=1361) ^ref-41281

---
It’s always worth making the effort to use static SQL that can be precompiled, rather than dynamic SQL that has to be compiled each time. Most platforms give you a mechanism for precompiling SQL. A good rule of thumb is to avoid using string concatenation to put together SQL queries. — location: [1365](kindle://book?action=open&asin=B008OHVDFM&location=1365) ^ref-591

---
There are two main forms of structuring a program in a Web server: as a script or as a server page. — location: [1383](kindle://book?action=open&asin=B008OHVDFM&location=1383) ^ref-31898

---
The script form is a program, usually with functions or methods to handle the HTTP call. — location: [1384](kindle://book?action=open&asin=B008OHVDFM&location=1384) ^ref-3710

---
You write the return page in HTML and insert into the HTML scriptlets of code to execute at certain points. Examples of this approach include PHP, ASP, and JSP. — location: [1393](kindle://book?action=open&asin=B008OHVDFM&location=1393) ^ref-7053

---
Because the script style works best for interpreting the request and the server page style works best for formatting a response, there’s the obvious option to use a script for request interpretation and a server page for response formatting. This separation is in fact an old idea that first surfaced in user interfaces with the pattern Model View Controller (330). — location: [1396](kindle://book?action=open&asin=B008OHVDFM&location=1396) ^ref-11823

---
As a result I prefer to use the term input controller for the controller in Model View Controller (330). — location: [1405](kindle://book?action=open&asin=B008OHVDFM&location=1405) ^ref-53899

---
A request comes in to an input controller, which pulls information off the request. It then forwards the business logic to an appropriate model object. The model object talks to the data source and does everything indicated by the request as well as gather information for the response. When it’s done it returns control to the input controller, which looks at the results and decides which view is needed to display the response. It then passes control, together with the response data, to the view. — location: [1409](kindle://book?action=open&asin=B008OHVDFM&location=1409) ^ref-27250

---
The first, and most important, reason for applying Model View Controller (330) is to ensure that the models are completely separated from the Web presentation. — location: [1414](kindle://book?action=open&asin=B008OHVDFM&location=1414) ^ref-37484

---
Putting the processing into separate Transaction Script (110) or Domain Model (116) objects will make it easier to test them as well. This is particularly important if you’re using a server page as your view. — location: [1416](kindle://book?action=open&asin=B008OHVDFM&location=1416) ^ref-61958

---
A lot of user-interface designs separate the presentation objects from the domain objects with an intermediate layer of Application Controller (379) objects. — location: [1419](kindle://book?action=open&asin=B008OHVDFM&location=1419) ^ref-43576

---
The purpose of an Application Controller (379) is to handle the flow of an application, deciding which screens should appear in which order. — location: [1421](kindle://book?action=open&asin=B008OHVDFM&location=1421) ^ref-19122

---
Not all systems need an Application Controller (379). They’re useful if your system has a lot of logic about the order of screens and the navigation between them. — location: [1426](kindle://book?action=open&asin=B008OHVDFM&location=1426) ^ref-48511

---
If the machine is in control of the screen flow, you need an Application Controller (379); if the user is in control, you don’t. — location: [1430](kindle://book?action=open&asin=B008OHVDFM&location=1430) ^ref-32730

---
On the view side there are three patterns to think about: Transform View (361), Template View (350), and Two Step View (365). — location: [1431](kindle://book?action=open&asin=B008OHVDFM&location=1431) ^ref-26994

---
essentially two choices: whether to use Transform View (361) or Template View (350), — location: [1434](kindle://book?action=open&asin=B008OHVDFM&location=1434) ^ref-15730

---
and whether either of them uses one stage or a Two Step View (365). — location: [1435](kindle://book?action=open&asin=B008OHVDFM&location=1435) ^ref-56107

---
The basic patterns for Transform View (361) and Template View (350) are single stage. Two Step View (365) is a variation you can apply to either. — location: [1436](kindle://book?action=open&asin=B008OHVDFM&location=1436) ^ref-40207

---
Template View (350) allows you write the presentation in the structure of the page and embed markers into the page to indicate where dynamic content needs to go. — location: [1440](kindle://book?action=open&asin=B008OHVDFM&location=1440) ^ref-11423

---
This clearly provides a lot of power and flexibility; sadly, it also leads to very messy code that’s difficult to maintain. — location: [1443](kindle://book?action=open&asin=B008OHVDFM&location=1443) ^ref-45074

---
The Transform View (361) uses a transform style of program. The usual example is XSLT. This can be very effective if you’re working with domain data that’s in XML format or can easily be converted to it. — location: [1445](kindle://book?action=open&asin=B008OHVDFM&location=1445) ^ref-37570

---
If you use procedural scripts as your view, you can write the code in the style of either Transform View (361) or Template View (350) — location: [1447](kindle://book?action=open&asin=B008OHVDFM&location=1447) ^ref-47875

---
A single-stage view mostly has one view component for each screen in the application. The view takes domain oriented data and renders it in HTML. — location: [1451](kindle://book?action=open&asin=B008OHVDFM&location=1451) ^ref-31031

---
The advantage of the Two Step View (365) is that it puts the decision of what HTML to use in a single place. — location: [1458](kindle://book?action=open&asin=B008OHVDFM&location=1458) ^ref-6087

---
Two Step View (365) works even better if you have a Web application where its services are being used by multiple front-end customers, such as multiple airlines fronting the same basic reservation system. Within the limits of the logical screen, each front end can have a different appearance by using a different second stage. — location: [1462](kindle://book?action=open&asin=B008OHVDFM&location=1462) ^ref-32974

---
There are two patterns for the input controller. The most common is an input controller object for every page on your Web site. In the simplest case this Page Controller (333) can be a server page itself, combining the roles of view and input controller. — location: [1468](kindle://book?action=open&asin=B008OHVDFM&location=1468) ^ref-19338

---
Often you’ll find that there isn’t quite a one-to-one relationship between Page Controllers (333) and views. — location: [1471](kindle://book?action=open&asin=B008OHVDFM&location=1471) ^ref-32396

---
A more precise thought is that you have a Page Controller (333) for each action, where an action is a button or link. — location: [1473](kindle://book?action=open&asin=B008OHVDFM&location=1473) ^ref-26917

---
With any input controller there are two responsibilities—handling the HTTP request and deciding what to do with it—and it often makes sense to separate them. A server page can handle the request, delegating a separate helper object to decide what to do with it. — location: [1475](kindle://book?action=open&asin=B008OHVDFM&location=1475) ^ref-10144

---
Front Controller (344) goes further in this separation by having only one object handling all requests. This single handler interprets the URL to figure out what kind of request it’s dealing with and creates a separate object to process it. — location: [1477](kindle://book?action=open&asin=B008OHVDFM&location=1477) ^ref-37889

---
The term we use is offline concurrency, that is, concurrency control for data that’s manipulated during multiple database transactions. — location: [1496](kindle://book?action=open&asin=B008OHVDFM&location=1496) ^ref-57494

---
An inconsistent read occurs when you read two things that are correct pieces of information but not correct at the same time. — location: [1514](kindle://book?action=open&asin=B008OHVDFM&location=1514) ^ref-50289

---
Both of these problems cause a failure of correctness (or safety), and they result in incorrect behavior that would not have occurred without two people trying to work with the same data at the same time. — location: [1522](kindle://book?action=open&asin=B008OHVDFM&location=1522) ^ref-47134

---
The essential problem of any concurrent programming is that it’s not enough to worry about correctness; you also have to worry about liveness: how much concurrent activity can go on. — location: [1525](kindle://book?action=open&asin=B008OHVDFM&location=1525) ^ref-9483

---
From the perspective of interacting with the outside world, two important contexts are the request and the session. — location: [1533](kindle://book?action=open&asin=B008OHVDFM&location=1533) ^ref-8573

---
A request corresponds to a single call from the outside world which the software works on and for which it optionally sends back a response. — location: [1534](kindle://book?action=open&asin=B008OHVDFM&location=1534) ^ref-16382

---
A session is a long-running interaction between a client and a server. It may consist of a single request, but more commonly it consists of a series of requests that the user regards as a consistent logical sequence. — location: [1539](kindle://book?action=open&asin=B008OHVDFM&location=1539) ^ref-48785

---
A process is a, usually heavyweight, execution context that provides a lot of isolation for the internal data it works on. — location: [1545](kindle://book?action=open&asin=B008OHVDFM&location=1545) ^ref-50752

---
A thread is a lighter-weight active agent that’s set up so that multiple threads can operate in a single process. — location: [1546](kindle://book?action=open&asin=B008OHVDFM&location=1546) ^ref-22547

---
However, threads usually share memory, and such sharing leads to concurrency problems. — location: [1548](kindle://book?action=open&asin=B008OHVDFM&location=1548) ^ref-57721

---
Some environments allow you to control what data a thread may access, allowing you to have isolated threads that don’t share memory. — location: [1549](kindle://book?action=open&asin=B008OHVDFM&location=1549) ^ref-58070

---
For enterprise applications two solutions are particularly important: isolation and immutability. — location: [1559](kindle://book?action=open&asin=B008OHVDFM&location=1559) ^ref-57847

---
Concurrency problems occur when more than one active agent, such as a process or thread, has access to the same piece of data. — location: [1560](kindle://book?action=open&asin=B008OHVDFM&location=1560) ^ref-62888

---
One way to deal with this is isolation: Partition the data so that any piece of it can only be accessed by one active agent. — location: [1561](kindle://book?action=open&asin=B008OHVDFM&location=1561) ^ref-22184

---
The operating system allocates memory exclusively to a single process, and only that process can read or write the data linked to it. — location: [1562](kindle://book?action=open&asin=B008OHVDFM&location=1562) ^ref-20062

---
Isolation is a vital technique because it reduces the chance of errors. — location: [1565](kindle://book?action=open&asin=B008OHVDFM&location=1565) ^ref-29266

---
With isolation you arrange things so that the program enters an isolated zone, within which you don’t have to worry about concurrency. — location: [1566](kindle://book?action=open&asin=B008OHVDFM&location=1566) ^ref-31238

---
You only get concurrency problems if the data you’re sharing can be modified. So one way to avoid concurrency conflicts is to recognize immutable data. — location: [1568](kindle://book?action=open&asin=B008OHVDFM&location=1568) ^ref-37052

---
Another option is to separate applications that are only reading data, and have them use copied data sources, from which we can then relax all concurrency controls. — location: [1571](kindle://book?action=open&asin=B008OHVDFM&location=1571) ^ref-50082

---
With optimistic locking both of them can make a copy of the file and edit it freely. If David is the first to finish, he can check in his work without trouble. The concurrency control kicks in when Martin tries to commit his changes. At this point the source code control system detects a conflict between Martin’s changes and David’s changes. Martin’s commit is rejected and it’s up to him to figure out how to deal with the situation. — location: [1575](kindle://book?action=open&asin=B008OHVDFM&location=1575) ^ref-64464

---
With pessimistic locking whoever checks out the file first prevents anyone else from editing it. So if Martin is first to check out, David can’t work with the file until Martin is finished with it and commits his changes. — location: [1578](kindle://book?action=open&asin=B008OHVDFM&location=1578) ^ref-59680

---
A good way of thinking about this is that an optimistic lock is about conflict detection while a pessimistic lock is about conflict prevention. — location: [1580](kindle://book?action=open&asin=B008OHVDFM&location=1580) ^ref-25687

---
The problem with the pessimistic lock is that it reduces concurrency. — location: [1583](kindle://book?action=open&asin=B008OHVDFM&location=1583) ^ref-43021

---
pick a victim, who has to throw away his work and his locks so the others can make progress. — location: [1627](kindle://book?action=open&asin=B008OHVDFM&location=1627) ^ref-55353

---
A similar approach is to give every lock a time limit. Once you hit that limit you lose your locks and your work—essentially becoming a victim. — location: [1628](kindle://book?action=open&asin=B008OHVDFM&location=1628) ^ref-54890

---
a transaction is a bounded sequence of work, with both start and endpoints well defined. — location: [1646](kindle://book?action=open&asin=B008OHVDFM&location=1646) ^ref-40305

---
Software transactions are often described in terms of the ACID properties: — location: [1652](kindle://book?action=open&asin=B008OHVDFM&location=1652) ^ref-28681

---
Atomicity: Each step in the sequence of actions performed within the boundaries of a transaction must complete successfully or all work must roll back. — location: [1654](kindle://book?action=open&asin=B008OHVDFM&location=1654) ^ref-28590

---
Consistency: A system’s resources must be in a consistent, noncorrupt state at both the start and the completion of a transaction. — location: [1658](kindle://book?action=open&asin=B008OHVDFM&location=1658) ^ref-51791

---
Isolation: The result of an individual transaction must not be visible to any other open transactions until that transaction commits successfully. — location: [1659](kindle://book?action=open&asin=B008OHVDFM&location=1659) ^ref-8399

---
Durability: Any result of a committed transaction must be made permanent. — location: [1660](kindle://book?action=open&asin=B008OHVDFM&location=1660) ^ref-44918

---
A variation on this is to open a transaction as late as possible. With a late transaction you may do all the reads outside it and only open it up when you do updates. This has the advantage of minimizing the time spent in a transaction. If there’s a lengthy time lag between the opening of the transaction and the first write, this may improve liveness. However, this means that you don’t have any concurrency control until you begin the transaction, which leaves you open to inconsistent reads. — location: [1671](kindle://book?action=open&asin=B008OHVDFM&location=1671) ^ref-46913

---
The start of the process is deciding which domain logic approach to go with. The three main contenders are Transaction Script (110), Table Module (125), and Domain Model (116). — location: [2087](kindle://book?action=open&asin=B008OHVDFM&location=2087) ^ref-63241

---
The simplest of the three patterns is Transaction Script (110). It fits with the procedural model that most people are still comfortable with. — location: [2092](kindle://book?action=open&asin=B008OHVDFM&location=2092) ^ref-11280

---
Its great failing is that it doesn’t deal well with complex business logic, being particularly susceptible to duplicate code. — location: [2095](kindle://book?action=open&asin=B008OHVDFM&location=2095) ^ref-44398

---
At the other end of the scale is the Domain Model (116). Hard-core — location: [2098](kindle://book?action=open&asin=B008OHVDFM&location=2098) ^ref-8021

---
Once you get used to working with a Domain Model (116) even simple problems can be tackled with ease. — location: [2102](kindle://book?action=open&asin=B008OHVDFM&location=2102) ^ref-55998

---
object models and relational models don’t fit well together. — location: [2110](kindle://book?action=open&asin=B008OHVDFM&location=2110) ^ref-3884

---
Of the three patterns Table Module (125) is the one whose star rises the most when you have tools that match it. — location: [2119](kindle://book?action=open&asin=B008OHVDFM&location=2119) ^ref-17139

---
The simplest Transaction Scripts (110) contain their own database logic, but I avoid that even in the simplest cases. — location: [2127](kindle://book?action=open&asin=B008OHVDFM&location=2127) ^ref-30052

---
With a Row Data Gateway (152) each record is read into an object with a clear and explicit interface. — location: [2132](kindle://book?action=open&asin=B008OHVDFM&location=2132) ^ref-23149

---
If your Domain Model (116) is fairly simple, say a couple of dozen classes that are pretty close to the database, then an Active Record (160) makes sense. — location: [2156](kindle://book?action=open&asin=B008OHVDFM&location=2156) ^ref-59585

---
Organizes business logic by procedures where each procedure handles a single request from the presentation. — location: [2320](kindle://book?action=open&asin=B008OHVDFM&location=2320) ^ref-22474

---
A Transaction Script organizes all this logic primarily as a single procedure, making calls directly to the database or through a thin database wrapper. Each transaction will have its own Transaction Script, although common subtasks can be broken into subprocedures. — location: [2325](kindle://book?action=open&asin=B008OHVDFM&location=2325) ^ref-24489

---
One of the benefits of this approach is that you don’t need to worry about what other transactions are doing. Your task is to get the input, interrogate the database, munge, and save your results to the database. — location: [2331](kindle://book?action=open&asin=B008OHVDFM&location=2331) ^ref-42053

---
At the very least put them in distinct subroutines; better still, put them in classes separate from those that handle presentation and data source. — location: [2334](kindle://book?action=open&asin=B008OHVDFM&location=2334) ^ref-14560

---
You can organize your Transaction Scripts into classes in two ways. The most common is to have several Transaction Scripts in a single class, where each class defines a subject area of related Transaction Scripts. — location: [2337](kindle://book?action=open&asin=B008OHVDFM&location=2337) ^ref-53101

---
The other way is to have each Transaction Script in its own class (Figure 9.1), using the Command pattern [Gang of Four]. In — location: [2339](kindle://book?action=open&asin=B008OHVDFM&location=2339) ^ref-10534

---
However, you’ll often find that instantiating a new object helps with threading issues as it makes it easier to isolate data. — location: [2343](kindle://book?action=open&asin=B008OHVDFM&location=2343) ^ref-10230

---
The glory of Transaction Script is its simplicity. — location: [2348](kindle://book?action=open&asin=B008OHVDFM&location=2348) ^ref-51474

---
Since the whole point is to handle one transaction, any common code tends to be duplicated. — location: [2351](kindle://book?action=open&asin=B008OHVDFM&location=2351) ^ref-6237

---
Many Transaction Script designs have scripts that operate directly on the database, putting SQL code in the procedure. Here I’m using a simple Table Data Gateway (144) to wrap the SQL queries. Since this example is so simple, I’m using a single gateway rather than one for each table. — location: [2383](kindle://book?action=open&asin=B008OHVDFM&location=2383) ^ref-27469

---
As a result I see two styles of Domain Model in the field. A simple Domain Model looks very much like the database design with mostly one domain object for each database table. — location: [2458](kindle://book?action=open&asin=B008OHVDFM&location=2458) ^ref-34779

---
A rich Domain Model can look different from the database design, with inheritance, strategies, and other [Gang of Four] patterns, and complex webs of small interconnected objects. — location: [2460](kindle://book?action=open&asin=B008OHVDFM&location=2460) ^ref-14567

---
simple Domain Model can use Active Record (160), whereas a rich Domain Model requires Data Mapper (165). — location: [2462](kindle://book?action=open&asin=B008OHVDFM&location=2462) ^ref-50669

---
You’ll notice that a guiding force of many layering patterns is to keep as few dependencies as possible between the domain model and other parts of the system. — location: [2465](kindle://book?action=open&asin=B008OHVDFM&location=2465) ^ref-41310

---
A Domain Model should use fine-grained objects with fine-grained interfaces. — location: [2495](kindle://book?action=open&asin=B008OHVDFM&location=2495) ^ref-44108

---
if you have simple not-null checks and a couple of sums to calculate, a Transaction Script (110) is a better bet. — location: [2516](kindle://book?action=open&asin=B008OHVDFM&location=2516) ^ref-16076

---
If you’re using Domain Model, my first choice for database interaction is Data Mapper (165). — location: [2521](kindle://book?action=open&asin=B008OHVDFM&location=2521) ^ref-52838

---
When you use Domain Model you may want to consider Service Layer (133) to give your Domain Model a more distinct API. — location: [2524](kindle://book?action=open&asin=B008OHVDFM&location=2524) ^ref-6145

---
An immediate thing to notice is that every class, in this small example (Figure 9.3) contains both behavior and data. — location: [2538](kindle://book?action=open&asin=B008OHVDFM&location=2538) ^ref-49624

---
A single instance that handles the business logic for all rows in a database table or view. — location: [2614](kindle://book?action=open&asin=B008OHVDFM&location=2614) ^ref-50734

---
Thus, if we have an Employee class, any instance of it corresponds to a particular employee. — location: [2618](kindle://book?action=open&asin=B008OHVDFM&location=2618) ^ref-31419

---
you often need considerable programmatic gymnastics to pull data in and out of the database, transforming between two different representations of the data. — location: [2622](kindle://book?action=open&asin=B008OHVDFM&location=2622) ^ref-32942

---
A Table Module organizes domain logic with one class per table in the database, and a single instance of a class contains the various procedures that will act on the data. The primary distinction with Domain Model (116) is that, if you have many orders, a Domain Model (116) will have one order object per order while a Table Module will have one object to handle all orders. — location: [2623](kindle://book?action=open&asin=B008OHVDFM&location=2623) ^ref-25865

---
Defines an application’s boundary with a layer of services that establishes a set of available operations and coordinates the application’s response in each operation. — location: [2778](kindle://book?action=open&asin=B008OHVDFM&location=2778) ^ref-47934

---
A Service Layer defines an application’s boundary [Cockburn PloP] and its set of available operations from the perspective of interfacing client layers. — location: [2784](kindle://book?action=open&asin=B008OHVDFM&location=2784) ^ref-40426

---
It encapsulates the application’s business logic, controlling transactions and coordinating responses in the implementation of its operations. — location: [2785](kindle://book?action=open&asin=B008OHVDFM&location=2785) ^ref-41845

---
Like Transaction Script (110) and Domain Model (116), Service Layer is a pattern for organizing business logic. Many designers, including me, like to divide “business logic” into two kinds: “domain logic,” having to do purely with the problem domain (such as strategies for calculating revenue recognition on a contract), and “application logic,” having to do with application responsibilities [Cockburn UC] (such as notifying contract administrators, and integrated applications, of revenue recognition calculations). — location: [2790](kindle://book?action=open&asin=B008OHVDFM&location=2790) ^ref-46238

---
But putting application logic into pure domain object classes has a couple of undesirable consequences. First, domain object classes are less reusable across applications if they implement application-specific logic and depend on application-specific packages. — location: [2797](kindle://book?action=open&asin=B008OHVDFM&location=2797) ^ref-29168

---
Second, commingling both kinds of logic in the same classes makes it harder to reimplement the application logic in, say, a workflow tool if that should ever become desirable. — location: [2799](kindle://book?action=open&asin=B008OHVDFM&location=2799) ^ref-14136

---
approach. In the domain facade approach a Service Layer is implemented as a set of thin facades over a Domain Model (116). The classes implementing the facades don’t implement any business logic. Rather, the Domain Model (116) implements all of the business logic. — location: [2803](kindle://book?action=open&asin=B008OHVDFM&location=2803) ^ref-40958

---
In the operation script approach a Service Layer is implemented as a set of thicker classes that directly implement application logic but delegate to encapsulated domain object classes for domain logic. — location: [2807](kindle://book?action=open&asin=B008OHVDFM&location=2807) ^ref-19100

---
A Service Layer is comprised of these application service classes, which should extend a Layer Supertype (475), abstracting their responsibilities and common behaviors. — location: [2811](kindle://book?action=open&asin=B008OHVDFM&location=2811) ^ref-51317

---
Identifying the operations needed on a Service Layer boundary is pretty straightforward. They’re determined by the needs of Service Layer clients, the most significant (and first) of which is typically a user interface. — location: [2826](kindle://book?action=open&asin=B008OHVDFM&location=2826) ^ref-59210

---
there’s almost always a one-to-one correspondence between CRUD use cases and Service Layer operations. — location: [2831](kindle://book?action=open&asin=B008OHVDFM&location=2831) ^ref-25106

---
The benefit of Service Layer is that it defines a common set of application operations available to many kinds of clients and it coordinates an application’s response in each operation. — location: [2858](kindle://book?action=open&asin=B008OHVDFM&location=2858) ^ref-44669

---
Thus, in an application with more than one kind of client of its business logic, and complex responses in its use cases involving multiple transactional resources, it makes a lot of sense to include a Service Layer with container-managed transactions, even in an undistributed architecture. — location: [2860](kindle://book?action=open&asin=B008OHVDFM&location=2860) ^ref-39961

---
You probably don’t need a Service Layer if your application’s business logic will only have one kind of client—say, a user interface—and its use case responses don’t involve multiple transactional resources. — location: [2863](kindle://book?action=open&asin=B008OHVDFM&location=2863) ^ref-45852

---
the application must respond by sending an e-mail notification of that event to a designated contract administrator and by publishing a message using message-oriented middleware to notify other integrated applications. — location: [2879](kindle://book?action=open&asin=B008OHVDFM&location=2879) ^ref-2415

---
An object that acts as a Gateway (466) to a database table. One instance handles all the rows in the table. — location: [2942](kindle://book?action=open&asin=B008OHVDFM&location=2942) ^ref-40471

---
Mixing SQL in application logic can cause several problems. — location: [2944](kindle://book?action=open&asin=B008OHVDFM&location=2944) ^ref-30770

---
A Table Data Gateway holds all the SQL for accessing a single table or view: selects, inserts, updates, and deletes. — location: [2946](kindle://book?action=open&asin=B008OHVDFM&location=2946) ^ref-60118

---
Other code calls its methods for all interaction with the database. — location: [2946](kindle://book?action=open&asin=B008OHVDFM&location=2946) ^ref-64744

---
Each method maps the input parameters into a SQL call and executes the SQL against a database connection. — location: [2948](kindle://book?action=open&asin=B008OHVDFM&location=2948) ^ref-20154

---
The Table Data Gateway is usually stateless, as its role is to push data back and forth. — location: [2949](kindle://book?action=open&asin=B008OHVDFM&location=2949) ^ref-17127

---
better alternative is to use a Data Transfer Object (401). It’s another object to create but one that may well be used elsewhere. — location: [2955](kindle://book?action=open&asin=B008OHVDFM&location=2955) ^ref-9656

---
A Table Data Gateway thus goes very well with Table Module — location: [2960](kindle://book?action=open&asin=B008OHVDFM&location=2960) ^ref-51072

---
If you’re using a Domain Model (116), you can have the Table Data Gateway return the appropriate domain object. The problem with this is that you then have bidirectional dependencies between the domain objects and the gateway. — location: [2963](kindle://book?action=open&asin=B008OHVDFM&location=2963) ^ref-46311

---
Most times when you use Table Data Gateway, you’ll have one for each table in the database. For very simple cases, however, you can have a single Table Data Gateway that handles all methods for all tables. — location: [2966](kindle://book?action=open&asin=B008OHVDFM&location=2966) ^ref-44747

---
You can also have one for views or even for interesting queries that aren’t kept in the database as views. — location: [2967](kindle://book?action=open&asin=B008OHVDFM&location=2967) ^ref-7832

---
Obviously, view-based Table Data Gateways often can’t update and so won’t have update behavior. — location: [2968](kindle://book?action=open&asin=B008OHVDFM&location=2968) ^ref-42377

---
I find that Table Data Gateway is probably the simplest database interface pattern to use, as it maps so nicely onto a database table or record type. — location: [2973](kindle://book?action=open&asin=B008OHVDFM&location=2973) ^ref-40804

---
I use it least with Domain Model (116) because I find that Data Mapper (165) gives a better isolation between the Domain Model (116) and the database. — location: [2974](kindle://book?action=open&asin=B008OHVDFM&location=2974) ^ref-64823

---
An object that acts as a Gateway (466) to a single record in a data source. There is one instance per row. — location: [3109](kindle://book?action=open&asin=B008OHVDFM&location=3109) ^ref-39084

---
if your in-memory objects have business logic of their own, adding the database manipulation code increases complexity. — location: [3112](kindle://book?action=open&asin=B008OHVDFM&location=3112) ^ref-34978

---
Testing is awkward too since, if your in-memory objects are tied to a database, tests are slower to run because of all the database access. — location: [3113](kindle://book?action=open&asin=B008OHVDFM&location=3113) ^ref-35952

---
A Row Data Gateway gives you objects that look exactly like the record in your record structure but can be accessed with the regular mechanisms of your programming language. All details of data source access are hidden behind this interface. — location: [3115](kindle://book?action=open&asin=B008OHVDFM&location=3115) ^ref-19523

---
A Row Data Gateway acts as an object that exactly mimics a single record, such as one database row. In it each column in the database becomes one field. — location: [3117](kindle://book?action=open&asin=B008OHVDFM&location=3117) ^ref-26225

---
This pattern holds the data about a row so that a client can then access the Row Data Gateway directly. — location: [3119](kindle://book?action=open&asin=B008OHVDFM&location=3119) ^ref-46717

---
This approach works particularly well for Transaction Scripts — location: [3120](kindle://book?action=open&asin=B008OHVDFM&location=3120) ^ref-22776

---
It’s often hard to tell the difference between a Row Data Gateway and an Active Record (160). The crux of the matter is whether there’s any domain logic present; if there is, you have an Active Record (160). — location: [3126](kindle://book?action=open&asin=B008OHVDFM&location=3126) ^ref-19180

---
A Row Data Gateway should contain only database access logic and no domain logic. — location: [3129](kindle://book?action=open&asin=B008OHVDFM&location=3129) ^ref-34232

---
Row Data Gateways tend to be somewhat tedious to write, but they’re a very good candidate for code generation based on a Metadata Mapping (306). This way all your database access code can be automatically built for you during your automated build process. — location: [3134](kindle://book?action=open&asin=B008OHVDFM&location=3134) ^ref-52127

---
The choice of Row Data Gateway often takes two steps: first whether to use a gateway at all and second whether to use Row Data Gateway or Table Data Gateway (144). — location: [3137](kindle://book?action=open&asin=B008OHVDFM&location=3137) ^ref-38221

---
use Row Data Gateway most often when I’m using a Transaction Script (110). — location: [3138](kindle://book?action=open&asin=B008OHVDFM&location=3138) ^ref-35330

---
If the mapping is simple, Active Record (160) does the same job without an additional layer of code. If the mapping is complex, Data Mapper (165) works better, as it’s better at decoupling the data structure from the domain objects because the domain objects don’t need to know the layout of the database. — location: [3142](kindle://book?action=open&asin=B008OHVDFM&location=3142) ^ref-35165

---
Interestingly, I’ve seen Row Data Gateway used very nicely with Data Mapper (165). Although this seems like extra work, it can be effective iff the Row Data Gateways are automatically generated from metadata while the Data Mappers (165) are done by hand. — location: [3149](kindle://book?action=open&asin=B008OHVDFM&location=3149) ^ref-57829

---
If we want to use the Row Data Gateway from a Domain Model (116), the domain objects need to get at the data from the gateway. — location: [3236](kindle://book?action=open&asin=B008OHVDFM&location=3236) ^ref-42463

---
Instead of copying the data to the domain object we can use the Row Data Gateway as a data holder for the domain object. — location: [3237](kindle://book?action=open&asin=B008OHVDFM&location=3237) ^ref-30497

---
Accessors on the domain logic can then delegate to the gateway for the data. Click here to view code image — location: [3241](kindle://book?action=open&asin=B008OHVDFM&location=3241) ^ref-26712

---
An object that wraps a row in a database table or view, encapsulates the database access, and adds domain logic on that data. — location: [3250](kindle://book?action=open&asin=B008OHVDFM&location=3250) ^ref-14797

---
An object carries both data and behavior. Much of this data is persistent and needs to be stored in a database. Active Record uses the most obvious approach, putting data access logic in the domain object. This way all people know how to read and write their data to and from the database. — location: [3251](kindle://book?action=open&asin=B008OHVDFM&location=3251) ^ref-7831

---
The essence of an Active Record is a Domain Model (116) in which the classes match very closely the record structure of an underlying database. — location: [3254](kindle://book?action=open&asin=B008OHVDFM&location=3254) ^ref-12168

---
Each Active Record is responsible for saving and loading to the database and also for any domain logic that acts on the data. — location: [3255](kindle://book?action=open&asin=B008OHVDFM&location=3255) ^ref-38765

---
The data structure of the Active Record should exactly match that of the database: one field in the class for each column in the table. Type the fields the way the SQL interface gives you the data—don’t do any conversion at this stage. — location: [3258](kindle://book?action=open&asin=B008OHVDFM&location=3258) ^ref-52195

---
You may consider Foreign Key Mapping (236), but you may also leave the foreign keys as they are. You can use views or tables with Active Record, although updates through views are obviously — location: [3260](kindle://book?action=open&asin=B008OHVDFM&location=3260) ^ref-40682

---
The Active Record class typically has methods that do the following: — location: [3262](kindle://book?action=open&asin=B008OHVDFM&location=3262) ^ref-45190

---
Construct an instance of the Active Record from a SQL result set row — location: [3263](kindle://book?action=open&asin=B008OHVDFM&location=3263) ^ref-37211

---
Construct a new instance for later insertion into the table — location: [3264](kindle://book?action=open&asin=B008OHVDFM&location=3264) ^ref-54360

---
Static finder methods to wrap commonly used SQL queries and return Active Record objects — location: [3265](kindle://book?action=open&asin=B008OHVDFM&location=3265) ^ref-24183

---
Update the database and insert into it the data in the Active Record — location: [3266](kindle://book?action=open&asin=B008OHVDFM&location=3266) ^ref-49630

---
Get and set the fields — location: [3267](kindle://book?action=open&asin=B008OHVDFM&location=3267) ^ref-9470

---
Implement some pieces of business logic — location: [3268](kindle://book?action=open&asin=B008OHVDFM&location=3268) ^ref-29941

---
if you ask for a related table, the getting method can return the appropriate Active Record, even if you aren’t using Identity Field (216) on the data structure (by doing a lookup). — location: [3269](kindle://book?action=open&asin=B008OHVDFM&location=3269) ^ref-57947

---
Active Record is very similar to Row Data Gateway (152). The principal difference is that a Row Data Gateway (152) contains only database access while an Active Record contains both data source and domain logic. — location: [3273](kindle://book?action=open&asin=B008OHVDFM&location=3273) ^ref-34441

---
Because of the close coupling between the Active Record and the database, I more often see static find methods in this pattern. However, there’s no reason that you can’t separate out the find methods into a separate class, as I discussed with Row Data Gateway (152), and that is better for testing. — location: [3276](kindle://book?action=open&asin=B008OHVDFM&location=3276) ^ref-59880

---
Active Record is a good choice for domain logic that isn’t too complex, such as creates, reads, updates, and deletes. Derivations and validations based on a single record work well in this structure. — location: [3280](kindle://book?action=open&asin=B008OHVDFM&location=3280) ^ref-40285

---
Their primary problem is that they work well only if the Active Record objects correspond directly to the database tables: an isomorphic schema. — location: [3284](kindle://book?action=open&asin=B008OHVDFM&location=3284) ^ref-25555

---
Another argument against Active Record is the fact that it couples the object design to the database design. This makes it more difficult to refactor either design as a project goes forward. — location: [3288](kindle://book?action=open&asin=B008OHVDFM&location=3288) ^ref-38423

---
Active Record is a good pattern to consider if you’re using Transaction Script — location: [3289](kindle://book?action=open&asin=B008OHVDFM&location=3289) ^ref-16407

---
A layer of Mappers (473) that moves data between objects and a database while keeping them independent of each other and the mapper itself. — location: [3353](kindle://book?action=open&asin=B008OHVDFM&location=3353) ^ref-41163

---
If the in-memory objects know about the relational database structure, changes in one tend to ripple to the other. — location: [3359](kindle://book?action=open&asin=B008OHVDFM&location=3359) ^ref-39961

---
The Data Mapper is a layer of software that separates the in-memory objects from the database. Its responsibility is to transfer data between the two and also to isolate them from each other. — location: [3360](kindle://book?action=open&asin=B008OHVDFM&location=3360) ^ref-38501

---
With Data Mapper the in-memory objects needn’t know even that there’s a database present; they need no SQL interface code, and certainly no knowledge of the database schema. — location: [3362](kindle://book?action=open&asin=B008OHVDFM&location=3362) ^ref-15540

---
If you are going to use Data Mapper at all you usually need more complicated cases. — location: [3369](kindle://book?action=open&asin=B008OHVDFM&location=3369) ^ref-32848

---
The whole layer of Data Mapper can be substituted, either for testing purposes or to allow a single domain layer to work with different databases. — location: [3377](kindle://book?action=open&asin=B008OHVDFM&location=3377) ^ref-12829

---
Mappers need a variety of strategies to handle classes that turn into multiple fields, classes that have multiple tables, classes with inheritance, — location: [3379](kindle://book?action=open&asin=B008OHVDFM&location=3379) ^ref-23574

---
When it comes to inserts and updates, the database mapping layer needs to understand what objects have changed, which new ones have been created, and which ones have been destroyed. — location: [3382](kindle://book?action=open&asin=B008OHVDFM&location=3382) ^ref-56119

---
Figure 10.3 suggests that a single request to a find method results in a single SQL query. This isn’t always true. Loading a typical order with multiple order lines may involve loading the order lines as well. — location: [3385](kindle://book?action=open&asin=B008OHVDFM&location=3385) ^ref-44543

---
An application can have one Data Mapper or several. If you’re hardcoding your mappers, it’s best to use one for each domain class or root of a domain hierarchy. — location: [3395](kindle://book?action=open&asin=B008OHVDFM&location=3395) ^ref-62061

---
If you’re using Metadata Mapping (306), you can get away with a single mapper class. — location: [3397](kindle://book?action=open&asin=B008OHVDFM&location=3397) ^ref-4399

---
With a large application it can be too much to have a single mapper with lots of find methods, so it makes sense to split these methods up by each domain class or head of the domain hierarchy. — location: [3398](kindle://book?action=open&asin=B008OHVDFM&location=3398) ^ref-50512

---
Either you can have a Registry (480) of Identity Maps (195), or you can have each finder hold an Identity Map (195) (providing there is only one finder per class per session). — location: [3402](kindle://book?action=open&asin=B008OHVDFM&location=3402) ^ref-48695

---
On occasion you may need the domain objects to invoke find methods on the Data Mapper. However, I’ve found that with a good Lazy Load (200) you can completely avoid this. — location: [3408](kindle://book?action=open&asin=B008OHVDFM&location=3408) ^ref-29059

---
You can solve this dilemma by using Separated Interface (476). Put any find methods needed by the domain code into an interface class that you can place in the domain package. — location: [3412](kindle://book?action=open&asin=B008OHVDFM&location=3412) ^ref-1723

---
One is to create the object with a rich constructor so that it’s at least created with all its mandatory data. The other is to create an empty object and then populate it with the mandatory data. — location: [3422](kindle://book?action=open&asin=B008OHVDFM&location=3422) ^ref-10694

---
One of the decisions you need to make concerns storing the information about how fields in domain objects are mapped to columns in the database. The simplest, and often best, way to do this is with explicit code, which requires a mapper class for each domain object. — location: [3434](kindle://book?action=open&asin=B008OHVDFM&location=3434) ^ref-57374

---
An alternative is to use Metadata Mapping (306), which stores the metadata as data, either in a class or in a separate file. — location: [3437](kindle://book?action=open&asin=B008OHVDFM&location=3437) ^ref-28034

---
The primary occasion for using Data Mapper is when you want the database schema and the object model to evolve independently. — location: [3440](kindle://book?action=open&asin=B008OHVDFM&location=3440) ^ref-17771

---
Data Mapper’s primary benefit is that when working on the domain model you can ignore the database, both in design and in the build and testing process. — location: [3442](kindle://book?action=open&asin=B008OHVDFM&location=3442) ^ref-31290

---
If you have fairly simple business logic, you probably won’t need a Domain Model (116) or a Data Mapper. — location: [3448](kindle://book?action=open&asin=B008OHVDFM&location=3448) ^ref-58726

---
If the domain model is pretty simple, and the database is under the domain model developers’ control, then it’s reasonable for the domain objects to access the database directly with Active Record (160). — location: [3452](kindle://book?action=open&asin=B008OHVDFM&location=3452) ^ref-15845

---
However, I’ve added an abstract mapper Layer Supertype (475) to indicate where I can pull out some common behavior. — location: [3467](kindle://book?action=open&asin=B008OHVDFM&location=3467) ^ref-48153

---
To allow domain objects to invoke finder behavior I can use Separated Interface (476) to separate the finder interfaces from the mappers — location: [3579](kindle://book?action=open&asin=B008OHVDFM&location=3579) ^ref-64434

---
Maintains a list of objects affected by a business transaction and coordinates the writing out of changes and the resolution of concurrency problems. — location: [3687](kindle://book?action=open&asin=B008OHVDFM&location=3687) ^ref-21515

---
When you’re pulling data in and out of a database, it’s important to keep track of what you’ve changed; otherwise, that data won’t be written back into the database. — location: [3688](kindle://book?action=open&asin=B008OHVDFM&location=3688) ^ref-32399

---
Similarly you have to insert new objects you create and remove any objects you delete. — location: [3690](kindle://book?action=open&asin=B008OHVDFM&location=3690) ^ref-26661

---
You can change the database with each change to your object model, but this can lead to lots of very small database calls, which ends up being very slow. Furthermore it requires you to have a transaction open for the whole interaction, — location: [3690](kindle://book?action=open&asin=B008OHVDFM&location=3690) ^ref-3837

---
A Unit of Work keeps track of everything you do during a business transaction that can affect the database. When you’re done, it figures out everything that needs to be done to alter the database as a result of your work. — location: [3694](kindle://book?action=open&asin=B008OHVDFM&location=3694) ^ref-890

---
As soon as you start doing something that may affect a database, you create a Unit of Work to keep track of the changes. — location: [3697](kindle://book?action=open&asin=B008OHVDFM&location=3697) ^ref-4163

---
Every time you create, change, or delete an object you tell the Unit of Work. — location: [3698](kindle://book?action=open&asin=B008OHVDFM&location=3698) ^ref-56499

---
You can also let it know about objects you’ve read so that it can check for inconsistent reads by verifying that none of the objects changed on the database during the business transaction. — location: [3698](kindle://book?action=open&asin=B008OHVDFM&location=3698) ^ref-51335

---
when it comes time to commit, the Unit of Work decides what to do. — location: [3700](kindle://book?action=open&asin=B008OHVDFM&location=3700) ^ref-4774

---
Application programmers never explicitly call methods for database updates. — location: [3703](kindle://book?action=open&asin=B008OHVDFM&location=3703) ^ref-44790

---
Of course for this to work the Unit of Work needs to know what objects it should keep track of. You can do this either by the caller doing it or by getting the object to tell the Unit of Work. — location: [3704](kindle://book?action=open&asin=B008OHVDFM&location=3704) ^ref-34618

---
With caller registration (Figure 11.1), the user of an object has to remember to register the object with the Unit of Work for changes. — location: [3706](kindle://book?action=open&asin=B008OHVDFM&location=3706) ^ref-20550

---
With object registration (Figure 11.2), the onus is removed from the caller. The usual trick here is to place registration methods in object methods. — location: [3711](kindle://book?action=open&asin=B008OHVDFM&location=3711) ^ref-29437

---
Loading an object from the database registers the object as clean; the setting methods register the object as dirty. — location: [3713](kindle://book?action=open&asin=B008OHVDFM&location=3713) ^ref-11736

---
This is a natural place for code generation to generate appropriate calls, — location: [3718](kindle://book?action=open&asin=B008OHVDFM&location=3718) ^ref-21130

---
Another technique I’ve seen is unit of work controller — location: [3723](kindle://book?action=open&asin=B008OHVDFM&location=3723) ^ref-54575

---
Here the Unit of Work handles all reads from the database and registers clean objects whenever they’re read. — location: [3724](kindle://book?action=open&asin=B008OHVDFM&location=3724) ^ref-22921

---
Rather than marking objects as dirty the Unit of Work takes a copy at read time and then compares the object at commit time. — location: [3725](kindle://book?action=open&asin=B008OHVDFM&location=3725) ^ref-61741

---
A hybrid approach is to take copies only of changed objects. — location: [3727](kindle://book?action=open&asin=B008OHVDFM&location=3727) ^ref-20710

---
However, there are other solutions, such as providing a transient constructor that doesn’t register with the Unit of Work or, better still, providing a Special Case (496)Unit of Work that does nothing with a commit. — location: [3732](kindle://book?action=open&asin=B008OHVDFM&location=3732) ^ref-9887

---
Objects need to be able to find their current Unit of Work. A good way to do this is with a thread-scoped Registry — location: [3743](kindle://book?action=open&asin=B008OHVDFM&location=3743) ^ref-44596

---
Another way is to pass the Unit of Work to objects that need it, either in method calls or when you create an object. — location: [3744](kindle://book?action=open&asin=B008OHVDFM&location=3744) ^ref-48190

---
Unit of Work makes an obvious point of handling batch updates. The idea behind a batch update is to send multiple SQL commands as a single unit so that they can be processed in a single remote call. — location: [3746](kindle://book?action=open&asin=B008OHVDFM&location=3746) ^ref-13760

---
The fundamental problem that Unit of Work deals with is keeping track of the various objects you’ve manipulated so that you know which ones you need to consider to synchronize your in-memory data with the database. — location: [3759](kindle://book?action=open&asin=B008OHVDFM&location=3759) ^ref-48787

---
Perhaps the simplest alternative is to explicitly save any object whenever you alter it. — location: [3762](kindle://book?action=open&asin=B008OHVDFM&location=3762) ^ref-5981

---
To avoid multiple database calls, you can leave all your updates to the end. — location: [3764](kindle://book?action=open&asin=B008OHVDFM&location=3764) ^ref-8112

---
Variables often work fine with a Transaction Script (110), but they can be very difficult with a Domain Model (116). — location: [3766](kindle://book?action=open&asin=B008OHVDFM&location=3766) ^ref-54884

---
Rather than keep objects in variables you can give each object a dirty flag that you set when the object changes. — location: [3768](kindle://book?action=open&asin=B008OHVDFM&location=3768) ^ref-54317

---
Then you need to find all the dirty objects at the end of your transaction and write them out. The value of this technique hinges on how easy it is to find the dirty objects. — location: [3769](kindle://book?action=open&asin=B008OHVDFM&location=3769) ^ref-9522

---
The great strength of Unit of Work is that it keeps all this information in one place. Once you have it working for you, you don’t have to remember to do much in order to keep track of your changes. — location: [3772](kindle://book?action=open&asin=B008OHVDFM&location=3772) ^ref-37203

---
An object that doesn’t contain all of the data you need but knows how to get it. — location: [3949](kindle://book?action=open&asin=B008OHVDFM&location=3949) ^ref-58724

---
There are four main ways you can implement Lazy Load: lazy initialization, virtual proxy, value holder, and ghost. — location: [3957](kindle://book?action=open&asin=B008OHVDFM&location=3957) ^ref-54345

---
Lazy initialization [Beck Patterns] is the simplest approach. The basic idea is that every access to the field checks first to see if it’s null. If so, it calculates the value of the field before returning the field. — location: [3958](kindle://book?action=open&asin=B008OHVDFM&location=3958) ^ref-51803

---
To make this work you have to ensure that the field is self-encapsulated, meaning that all access to the field, even from within the class, is done through a getting method. — location: [3960](kindle://book?action=open&asin=B008OHVDFM&location=3960) ^ref-49098

---
Using lazy initialization is simple, but it does tend to force a dependency between the object and the database. — location: [3963](kindle://book?action=open&asin=B008OHVDFM&location=3963) ^ref-60466

---
works best for Active Record (160), Table Data Gateway (144), and Row Data Gateway (152). — location: [3964](kindle://book?action=open&asin=B008OHVDFM&location=3964) ^ref-36334

---
A virtual proxy is an object that looks like the object that should be in the field, but doesn’t actually contain anything. — location: [3968](kindle://book?action=open&asin=B008OHVDFM&location=3968) ^ref-27597

---
Only when one of its methods is called does it load the correct object from the database. — location: [3969](kindle://book?action=open&asin=B008OHVDFM&location=3969) ^ref-64090

---
The good thing about a virtual proxy is that it looks exactly like the object that’s supposed to be there. — location: [3969](kindle://book?action=open&asin=B008OHVDFM&location=3969) ^ref-46268

---
The bad thing is that it isn’t that object, so you can easily run into a nasty identity problem. Furthermore you can have more than one virtual proxy for the same real object. — location: [3970](kindle://book?action=open&asin=B008OHVDFM&location=3970) ^ref-48544

---
These problem don’t hit you if you only use virtual proxies for collections classes, such as lists. Since collections are Value Objects (486), their identity doesn’t matter. — location: [3976](kindle://book?action=open&asin=B008OHVDFM&location=3976) ^ref-32742

---
With domain classes you can get around these problems by using a value holder. This concept, which I first came across in Smalltalk, is an object that wraps some other object. To get the underlying object you ask the value holder for its value, but only on the first access does it pull the data from the database. — location: [3978](kindle://book?action=open&asin=B008OHVDFM&location=3978) ^ref-24381

---
ghost is the real object in a partial state. When you load the object from the database it contains just its ID. Whenever you try to access a field it loads its full state. Think of a ghost as an object, where every field is lazy-initialized in one fell swoop, or as a virtual proxy, where the object is its own virtual proxy. — location: [3983](kindle://book?action=open&asin=B008OHVDFM&location=3983) ^ref-15581

---
A virtual proxy/ghost doesn’t need to be completely devoid of data. If you have some data that’s quick to get hold of and commonly used, it may make sense to load it when you load the proxy or ghost. (This is sometimes referred to as a “light object.”) — location: [3987](kindle://book?action=open&asin=B008OHVDFM&location=3987) ^ref-45660

---
That means it’s usually only worth considering Lazy Load if the field requires an extra database call to access. — location: [4012](kindle://book?action=open&asin=B008OHVDFM&location=4012) ^ref-27456

---
Identity Field — location: [4218](kindle://book?action=open&asin=B008OHVDFM&location=4218) ^ref-26515

---
Reading data from a database is all very well, but in order to write data back you need to tie the database to the in-memory object system. — location: [4222](kindle://book?action=open&asin=B008OHVDFM&location=4222) ^ref-6401

---
The first concern is whether to use meaningful or meaningless keys. A meaningful key is something like the U.S. Social Security number for identifying a person. A meaningless key is essentially a random number the database dreams up that’s never intended for human use. — location: [4229](kindle://book?action=open&asin=B008OHVDFM&location=4229) ^ref-26423

---
To work at all, keys need to be unique; to work well, they need to be immutable. — location: [4232](kindle://book?action=open&asin=B008OHVDFM&location=4232) ^ref-54084

---
meaningful keys should be distrusted. — location: [4235](kindle://book?action=open&asin=B008OHVDFM&location=4235) ^ref-42047

---
A simple key uses only one database field; a compound key uses more than one. — location: [4237](kindle://book?action=open&asin=B008OHVDFM&location=4237) ^ref-5348

---
A good example is orders and line items, where a good key for the line item is a compound of the order number and a sequence number makes a good key for a line item. — location: [4238](kindle://book?action=open&asin=B008OHVDFM&location=4238) ^ref-18357

---
You have to choose the type of the key. The most common operation you’ll do with a key is equality checking, so you want a type with a fast equality operation. The other important operation is getting the next key. Hence a long integer type is often the best bet. — location: [4243](kindle://book?action=open&asin=B008OHVDFM&location=4243) ^ref-52142

---
You can have keys that are unique to the table or unique database-wide. A table-unique key is unique across the table, which is what you need for a key in any case. A database-unique key is unique across every row in every table in the database. A table-unique key is usually fine, but a database-unique key is often easier to do and allows you to use a single Identity Map — location: [4248](kindle://book?action=open&asin=B008OHVDFM&location=4248) ^ref-60059

---
The simplest form of Identity Field is a field that matches the type of the key in the database. — location: [4260](kindle://book?action=open&asin=B008OHVDFM&location=4260) ^ref-28863

---
Compound keys are more problematic. The best bet with them is to make a key class. A generic key class can store a sequence of objects that act as the elements of the key. — location: [4261](kindle://book?action=open&asin=B008OHVDFM&location=4261) ^ref-60261

---
If you use the same basic structure for all keys, you can do all of the key handling in a Layer Supertype (475). You can put default behavior that will work for most cases in the Layer Supertype (475) and extend it for the exceptional cases in the particular subtypes. — location: [4263](kindle://book?action=open&asin=B008OHVDFM&location=4263) ^ref-63007

---
A better approach is to use a separate key table. This table is typically one with two columns: name and next available value. — location: [4296](kindle://book?action=open&asin=B008OHVDFM&location=4296) ^ref-39404

---
you use a key table, it’s a good idea to design it so that access to it is in a separate transaction from the one that updates the table — location: [4300](kindle://book?action=open&asin=B008OHVDFM&location=4300) ^ref-30039

---
For a small object with value semantics, such as a money or date range object that won’t have its own table, it’s better to use Embedded Value (268). — location: [4318](kindle://book?action=open&asin=B008OHVDFM&location=4318) ^ref-50438

---
For a complex graph of objects that doesn’t need to be queried within the relational database, Serialized LOB (272) is usually easier to write and gives faster performance. — location: [4319](kindle://book?action=open&asin=B008OHVDFM&location=4319) ^ref-17468

---
An object that’s been created in memory but not saved to the database will not have a value for its key. — location: [4331](kindle://book?action=open&asin=B008OHVDFM&location=4331) ^ref-20271

---
If you want database-unique keys, you’ll only need one row, if you want table-unique keys, you’ll need one row per table. — location: [4366](kindle://book?action=open&asin=B008OHVDFM&location=4366) ^ref-30279

---
We need to ensure that no auto-commit is going on since we absolutely must have the select and update operating in one transaction. — location: [4378](kindle://book?action=open&asin=B008OHVDFM&location=4378) ^ref-9075

---
Foreign Key Mapping Maps an association between objects to a foreign key reference between tables. — location: [4648](kindle://book?action=open&asin=B008OHVDFM&location=4648) ^ref-60077

---
A Foreign Key Mapping maps an object reference to a foreign key in the database. — location: [4655](kindle://book?action=open&asin=B008OHVDFM&location=4655) ^ref-56052

---
(216). Each object contains the database key from the appropriate database table. If two objects are linked together with an association, this association can be replaced by a foreign key in the database. — location: [4656](kindle://book?action=open&asin=B008OHVDFM&location=4656) ^ref-45694

---
How can you tell what alterations to put in the database? Essentially you have three options: (1) delete and insert, (2) add a back pointer, and (3) diff the collection. — location: [4664](kindle://book?action=open&asin=B008OHVDFM&location=4664) ^ref-48694

---
With delete and insert you delete all the tracks in the database that link to the album, and then insert all the ones currently on the album. — location: [4668](kindle://book?action=open&asin=B008OHVDFM&location=4668) ^ref-46644

---
Adding a back pointer puts a link from the track back to the album, effectively making the association bidirectional. — location: [4672](kindle://book?action=open&asin=B008OHVDFM&location=4672) ^ref-28430

---
There are two possibilities here: diff with the current state of the database or diff with what you read the first time. — location: [4674](kindle://book?action=open&asin=B008OHVDFM&location=4674) ^ref-52997

---
Diffing with the database involves rereading the collection back from the database and then comparing the collection you read with the collection in the album. — location: [4675](kindle://book?action=open&asin=B008OHVDFM&location=4675) ^ref-22811

---
Diffing with what you read in the first place means that you have to keep what you read. This is better as it avoids another database read. — location: [4678](kindle://book?action=open&asin=B008OHVDFM&location=4678) ^ref-2401

---
In the general case anything that’s added to the collection needs to be checked first to see if it’s a new object. You can do this by seeing if it has a key; if it doesn’t, one needs to be added to the database. — location: [4680](kindle://book?action=open&asin=B008OHVDFM&location=4680) ^ref-60487

---
If the link is immutable, meaning that you can’t change a track’s album, then adding always means insertion and removing always means deletion. — location: [4688](kindle://book?action=open&asin=B008OHVDFM&location=4688) ^ref-59881

---
A Foreign Key Mapping can be used for almost all associations between classes. The most common case where it isn’t possible is with many-to-many associations. — location: [4700](kindle://book?action=open&asin=B008OHVDFM&location=4700) ^ref-49476

---
Association Table Mapping — location: [4849](kindle://book?action=open&asin=B008OHVDFM&location=4849) ^ref-34010

---
The link table has no corresponding in-memory object. As a result it has no ID. — location: [4859](kindle://book?action=open&asin=B008OHVDFM&location=4859) ^ref-55408

---
Some objects naturally appear in the context of other objects. Tracks on an album may be loaded or saved whenever the underlying album is loaded or saved. If they aren’t referenced to by any other table in the database, you can simplify the mapping procedure by having the album mapper perform the mapping for the tracks as well—treating this mapping as a dependent mapping. — location: [5144](kindle://book?action=open&asin=B008OHVDFM&location=5144) ^ref-40658

---
The basic idea behind Dependent Mapping is that one class (the dependent) relies upon some other class (the owner) for its database persistence. Each dependent can have only one owner and must have one owner. — location: [5147](kindle://book?action=open&asin=B008OHVDFM&location=5147) ^ref-26290

---
If the dependents are expensive to load and infrequently used, you can use a Lazy Load (200) to avoid loading the dependents until you need them. — location: [5154](kindle://book?action=open&asin=B008OHVDFM&location=5154) ^ref-51478

---
An important property of a dependent is that it doesn’t have an Identity Field (216) and therefore isn’t stored in a Identity Map (195). — location: [5156](kindle://book?action=open&asin=B008OHVDFM&location=5156) ^ref-59438

---
Indeed, there’s no finder for a dependent since all finds are done with the owner. — location: [5158](kindle://book?action=open&asin=B008OHVDFM&location=5158) ^ref-577

---
A dependent may itself be the owner of another dependent. In this case the owner of the first dependent is also responsible for the persistence of the second dependent. — location: [5159](kindle://book?action=open&asin=B008OHVDFM&location=5159) ^ref-21474

---
You can have a whole hierarchy of dependents controlled by a single primary owner. — location: [5160](kindle://book?action=open&asin=B008OHVDFM&location=5160) ^ref-64896

---
No other table should have a foreign key into the dependent’s table, unless that object has the same owner. — location: [5161](kindle://book?action=open&asin=B008OHVDFM&location=5161) ^ref-62408

---
no in-memory object other than the owner or its dependents should have a reference to a dependent. — location: [5162](kindle://book?action=open&asin=B008OHVDFM&location=5162) ^ref-5397

---
Since the writing and saving of dependents is left to the owner, and there are no outside references, updates to the dependents can be handled through deletion and insertion. — location: [5165](kindle://book?action=open&asin=B008OHVDFM&location=5165) ^ref-7964

---
if you want to update the collection of dependents you can safely delete all rows that link to the owner and then reinsert all the dependents. — location: [5166](kindle://book?action=open&asin=B008OHVDFM&location=5166) ^ref-4964

---
Dependents are in many ways like Value Objects (486), although they often don’t need the full mechanics that you use in making something a Value Object (486) (such as overriding equals). The main difference is that there’s nothing special about them from a purely in-memory point of view. — location: [5168](kindle://book?action=open&asin=B008OHVDFM&location=5168) ^ref-40173

---
Using Dependent Mapping complicates tracking whether the owner has changed. Any change to a dependent needs to mark the owner as changed so that the owner will write the changes out to the database. — location: [5172](kindle://book?action=open&asin=B008OHVDFM&location=5172) ^ref-27610

---
You can simplify this considerably by making the dependent immutable, so that any change to it needs to be done by removing it and adding a new one. — location: [5173](kindle://book?action=open&asin=B008OHVDFM&location=5173) ^ref-34994

---
You use Dependent Mapping when you have an object that’s only referred to by one other object, which usually occurs when one object has a collection of dependents. — location: [5177](kindle://book?action=open&asin=B008OHVDFM&location=5177) ^ref-22506

---
A dependent must have exactly one owner. — location: [5181](kindle://book?action=open&asin=B008OHVDFM&location=5181) ^ref-47592

---
There must be no references from any object other than the owner to the dependent. — location: [5182](kindle://book?action=open&asin=B008OHVDFM&location=5182) ^ref-38202

---
Maps an object into several fields of another object’s table. — location: [5250](kindle://book?action=open&asin=B008OHVDFM&location=5250) ^ref-44595

---
An Embedded Value maps the values of an object to fields in the record of the object’s owner. — location: [5253](kindle://book?action=open&asin=B008OHVDFM&location=5253) ^ref-2363

---
Saves a graph of objects by serializing them into a single large object (LOB), which it stores in a database field. — location: [5316](kindle://book?action=open&asin=B008OHVDFM&location=5316) ^ref-61487

---
The basic schema is simple—an organization table with a parent foreign key, however, its manipulation of the schema requires many joins, which are both slow and awkward. — location: [5322](kindle://book?action=open&asin=B008OHVDFM&location=5322) ^ref-36121

---
Objects don’t have to be persisted as table rows related to each other. Another form of persistence is serialization, where a whole graph of objects is written out as a single large object (LOB) in a table this Serialized LOB then becomes a form of memento — location: [5323](kindle://book?action=open&asin=B008OHVDFM&location=5323) ^ref-34027

---
There are two ways you can do the serialization: as a binary (BLOB) or as textual characters (CLOB). — location: [5326](kindle://book?action=open&asin=B008OHVDFM&location=5326) ^ref-47537

---
Serialized LOB isn’t considered as often as it might be. XML makes it much more attractive since it yields a easy-to-implement textual approach. Its main disadvantage is that you can’t query the structure using SQL. — location: [5348](kindle://book?action=open&asin=B008OHVDFM&location=5348) ^ref-2023

---
This pattern works best when you can chop out a piece of the object model and use it to represent the LOB. Think of a LOB as a way to take a bunch of objects that aren’t likely to be queried from any SQL route outside the application. This graph can then be hooked into the SQL schema. — location: [5350](kindle://book?action=open&asin=B008OHVDFM&location=5350) ^ref-45623

---
Represents an inheritance hierarchy of classes as a single table that has columns for all the fields of the various classes. — location: [5417](kindle://book?action=open&asin=B008OHVDFM&location=5417) ^ref-25587

---
Relational databases don’t support inheritance, so when mapping from objects to databases we have to consider how to represent our nice inheritance structures in relational tables. — location: [5418](kindle://book?action=open&asin=B008OHVDFM&location=5418) ^ref-61365

---
Single Table Inheritance maps all fields of all classes of an inheritance structure into a single table. — location: [5421](kindle://book?action=open&asin=B008OHVDFM&location=5421) ^ref-52105

---
In this inheritance mapping scheme we have one table that contains all the data for all the classes in the inheritance hierarchy. — location: [5422](kindle://book?action=open&asin=B008OHVDFM&location=5422) ^ref-61301

---
When loading an object into memory you need to know which class to instantiate. For this you have a field in the table that indicates which class should be used. This can be the name of the class or a code field. — location: [5425](kindle://book?action=open&asin=B008OHVDFM&location=5425) ^ref-65060

---
Single Table Inheritance is one of the options for mapping the fields in an inheritance hierarchy to a relational database. — location: [5431](kindle://book?action=open&asin=B008OHVDFM&location=5431) ^ref-46221

---
There’s only a single table to worry about on the database. • There are no joins in retrieving data. • Any refactoring that pushes fields up or down the hierarchy doesn’t require you to change the database. — location: [5435](kindle://book?action=open&asin=B008OHVDFM&location=5435) ^ref-23525

---
Fields are sometimes relevant and sometimes not, which can be confusing to people using the tables directly. — location: [5438](kindle://book?action=open&asin=B008OHVDFM&location=5438) ^ref-4420

---
Columns used only by some subclasses lead to wasted space in the database. — location: [5439](kindle://book?action=open&asin=B008OHVDFM&location=5439) ^ref-58462

---
The single table may end up being too large, with many indexes and frequent locking, which may hurt performance. — location: [5442](kindle://book?action=open&asin=B008OHVDFM&location=5442) ^ref-42259

---
You only have a single namespace for fields, so you have to be sure that you don’t use the same name for different fields. — location: [5444](kindle://book?action=open&asin=B008OHVDFM&location=5444) ^ref-22732

---
Represents an inheritance hierarchy of classes with one table for each class. — location: [5554](kindle://book?action=open&asin=B008OHVDFM&location=5554) ^ref-37572

---
The biggest implementation issue with Class Table Inheritance is how to bring the data back from multiple tables in an efficient manner. — location: [5565](kindle://book?action=open&asin=B008OHVDFM&location=5565) ^ref-16019

---
You can avoid this by doing a join across the various component tables; however, joins for more than three or four tables tend to be slow because of the way databases do their optimizations. — location: [5567](kindle://book?action=open&asin=B008OHVDFM&location=5567) ^ref-18934

---
Class Table Inheritance, Single Table Inheritance (278) and Concrete Table Inheritance (293) are the three alternatives to consider for inheritance mapping. — location: [5572](kindle://book?action=open&asin=B008OHVDFM&location=5572) ^ref-59489

---
You need to pay attention to the keys with this pattern. Punningly, the key thing is to ensure that keys are unique not just to a table but to all the tables from a hierarchy. — location: [5710](kindle://book?action=open&asin=B008OHVDFM&location=5710) ^ref-33220

---
A structure to organize database mappers that handle inheritance hierarchies. — location: [5859](kindle://book?action=open&asin=B008OHVDFM&location=5859) ^ref-20314

---
You can organize the mappers with a hierarchy so that each domain class has a mapper that saves and loads the data for that domain class. — location: [5866](kindle://book?action=open&asin=B008OHVDFM&location=5866) ^ref-43216

---
A Metadata Mapping allows developers to define the mappings in a simple tabular form, which can then be processed by generic code to carry out the details of reading, inserting, and updating the data. — location: [5903](kindle://book?action=open&asin=B008OHVDFM&location=5903) ^ref-54536

---
There are two main routes to take: code generation and reflective programming. — location: [5906](kindle://book?action=open&asin=B008OHVDFM&location=5906) ^ref-13860

---
With code generation you write a program whose input is the metadata and whose output is the source code of classes that do the mapping. — location: [5906](kindle://book?action=open&asin=B008OHVDFM&location=5906) ^ref-12095

---
If you use code generation, you should make sure that it’s fully integrated into your build process with whatever build scripts you’re using. — location: [5909](kindle://book?action=open&asin=B008OHVDFM&location=5909) ^ref-4433

---
Reflective programming often suffers in speed, although the problem here depends very much on the actual environment you’re using— — location: [5920](kindle://book?action=open&asin=B008OHVDFM&location=5920) ^ref-36750

---
Remember, though, that the reflection is being done in the context of an SQL call, so its slower speed may not make that much difference considering the slow speed of the remote call. — location: [5921](kindle://book?action=open&asin=B008OHVDFM&location=5921) ^ref-21131

---
On most occasions you keep the metadata in a separate file format. These days XML is a popular choice as it provides hierarchic structuring while freeing you from writing your own parsers and other tools. — location: [5926](kindle://book?action=open&asin=B008OHVDFM&location=5926) ^ref-21497

---
In simpler cases you can skip the external file format and create the metadata representation directly in source code. This saves you from having to parse, but it makes editing the metadata somewhat harder. — location: [5929](kindle://book?action=open&asin=B008OHVDFM&location=5929) ^ref-45643

---
If you use reflective programming, you’ll typically access and parse during execution but only once during system startup; then you can keep the in-memory representation. — location: [5933](kindle://book?action=open&asin=B008OHVDFM&location=5933) ^ref-60138

---
To handle these minority cases you often have to add a lot of complexity to metadata. A useful alternative is to override the generic code with subclasses where the special code is handwritten. — location: [5939](kindle://book?action=open&asin=B008OHVDFM&location=5939) ^ref-369

---
Metadata Mapping can greatly reduce the amount of work needed to handle database mapping. — location: [5944](kindle://book?action=open&asin=B008OHVDFM&location=5944) ^ref-48895

---
If you’re building your own system, you should evaluate the trade-offs yourself. Compare adding new mappings using handwritten code with using Metadata Mapping. — location: [5948](kindle://book?action=open&asin=B008OHVDFM&location=5948) ^ref-11248

---
If you use reflection, look into its consequences for performance; — location: [5949](kindle://book?action=open&asin=B008OHVDFM&location=5949) ^ref-1767

---
The extra work of hand-coding can be greatly reduced by creating a good Layer Supertype (475) that handles all the common behavior. — location: [5950](kindle://book?action=open&asin=B008OHVDFM&location=5950) ^ref-29975

---
An object that represents a database query. — location: [6103](kindle://book?action=open&asin=B008OHVDFM&location=6103) ^ref-30476

---
A Query Object is an interpreter [Gang of Four], that is, a structure of objects that can form itself into a SQL query. — location: [6107](kindle://book?action=open&asin=B008OHVDFM&location=6107) ^ref-57633

---
A Query Object is an application of the Interpreter pattern geared to represent a SQL query. — location: [6110](kindle://book?action=open&asin=B008OHVDFM&location=6110) ^ref-48463

---
In order to represent any query, you need a flexible Query Object. — location: [6112](kindle://book?action=open&asin=B008OHVDFM&location=6112) ^ref-17488

---
common feature of Query Object is that it can represent queries in the language of the in-memory objects rather than the database schema. — location: [6116](kindle://book?action=open&asin=B008OHVDFM&location=6116) ^ref-2970

---
the Query Object needs to know how the database structure maps to the object structure, a capability that really needs Metadata Mapping — location: [6119](kindle://book?action=open&asin=B008OHVDFM&location=6119) ^ref-17800

---
For multiple databases you can design your Query Object so that it produces different SQL depending on which database the query is running against. — location: [6121](kindle://book?action=open&asin=B008OHVDFM&location=6121) ^ref-2575

---
A particularly sophisticated use of Query Object is to eliminate redundant queries against a database. — location: [6123](kindle://book?action=open&asin=B008OHVDFM&location=6123) ^ref-41867

---
If you see that you’ve run the same query earlier in a session, you can use it to select objects from the Identity Map (195) and avoid a trip to the database. — location: [6124](kindle://book?action=open&asin=B008OHVDFM&location=6124) ^ref-25508

---
A variation on the Query Object is to allow a query to be specified by an example domain object. Thus, — location: [6128](kindle://book?action=open&asin=B008OHVDFM&location=6128) ^ref-40427

---
Mediates between the domain and data mapping layers using a collection-like interface for accessing domain objects. — location: [6215](kindle://book?action=open&asin=B008OHVDFM&location=6215) ^ref-34047

---
A Repository mediates between the domain and data mapping layers, acting like an in-memory domain object collection. — location: [6221](kindle://book?action=open&asin=B008OHVDFM&location=6221) ^ref-2336

---
Conceptually, a Repository encapsulates the set of objects persisted in a data store and the operations performed over them, providing a more object-oriented view of the persistence layer. Repository also supports the objective of achieving a clean separation and one-way dependency between the domain and data mapping layers. — location: [6224](kindle://book?action=open&asin=B008OHVDFM&location=6224) ^ref-17435

---
A centralized point for handling screen navigation and the flow of an application. — location: [7230](kindle://book?action=open&asin=B008OHVDFM&location=7230) ^ref-37004

---
You can remove this duplication by placing all the flow logic in an Application Controller. Input controllers then ask the Application Controller for the appropriate commands for execution against a model and the correct view to use depending on the application context. — location: [7237](kindle://book?action=open&asin=B008OHVDFM&location=7237) ^ref-15714

---
Data Transfer Object An object that carries data between processes in order to reduce the number of method calls. — location: [7625](kindle://book?action=open&asin=B008OHVDFM&location=7625) ^ref-34757

---
Gateway An object that encapsulates access to an external system or resource. — location: [8774](kindle://book?action=open&asin=B008OHVDFM&location=8774) ^ref-26129

---
Not only does this make the software harder to understand, it also makes it much harder to change should you shift some data from a relational database to an XML message at some point in the future. — location: [8780](kindle://book?action=open&asin=B008OHVDFM&location=8780) ^ref-50292

---
Wrap all the special API code into a class whose interface looks like a regular object. Other objects access the resource through this Gateway, — location: [8782](kindle://book?action=open&asin=B008OHVDFM&location=8782) ^ref-969

---
Take the external resource. What does the application need to do with it? Create a simple API for your usage and use the Gateway to translate to the external source. — location: [8784](kindle://book?action=open&asin=B008OHVDFM&location=8784) ^ref-37511

---
Keep a Gateway as simple as you can. Focus on the essential roles of adapting the external service and providing a good point for stubbing. — location: [8789](kindle://book?action=open&asin=B008OHVDFM&location=8789) ^ref-12035

---
Often it’s a good idea to use code generation to create Gateways. — location: [8791](kindle://book?action=open&asin=B008OHVDFM&location=8791) ^ref-10846

---
You should consider Gateway whenever you have an awkward interface to something that feels external. Rather than let the awkwardness spread through the whole system, use a Gateway to contain it. — location: [8800](kindle://book?action=open&asin=B008OHVDFM&location=8800) ^ref-9889

---
A clear benefit of Gateway is that it also makes it easier for you to swap out one kind of resource for another. — location: [8805](kindle://book?action=open&asin=B008OHVDFM&location=8805) ^ref-17305

---
that even if you don’t think the resource is ever going to change, you can benefit from the simplicity and testability Gateway gives you. — location: [8808](kindle://book?action=open&asin=B008OHVDFM&location=8808) ^ref-33105

---
However, Mapper (473) is more complicated than Gateway. — location: [8810](kindle://book?action=open&asin=B008OHVDFM&location=8810) ^ref-25714

---
While Facade simplifies a more complex API, it’s usually done by the writer of the service for general use. A Gateway is written by the client for its particular use. — location: [8814](kindle://book?action=open&asin=B008OHVDFM&location=8814) ^ref-44658

---
Adapter alters an implementation’s interface to match another interface you need to work with. — location: [8817](kindle://book?action=open&asin=B008OHVDFM&location=8817) ^ref-64544

---
Mediator usually separates multiple objects so that they don’t know about each other but do know about the mediator. — location: [8820](kindle://book?action=open&asin=B008OHVDFM&location=8820) ^ref-64309

---
method. It’s the gateway’s role to make a more convenient interface. — location: [8840](kindle://book?action=open&asin=B008OHVDFM&location=8840) ^ref-56918

---
We can test objects that use the gateway without the message-sending service being present. To do this we need to create a Service Stub (504). In this case the gateway stub is a subclass of the real gateway and overrides doSend. — location: [8868](kindle://book?action=open&asin=B008OHVDFM&location=8868) ^ref-48426

---
Mapper An object that sets up a communication between two independent objects. — location: [8902](kindle://book?action=open&asin=B008OHVDFM&location=8902) ^ref-50782

---
A mapper is an insulating layer between subsystems. It controls the details of the communication between them without either subsystem being aware of it. — location: [8906](kindle://book?action=open&asin=B008OHVDFM&location=8906) ^ref-34708

---
The complicated part of using a mapper is deciding how to invoke it, since it can’t be directly invoked by either of the subsystems that it’s mapping between. Sometimes a third subsystem drives the mapping and invokes the mapper as well. — location: [8908](kindle://book?action=open&asin=B008OHVDFM&location=8908) ^ref-62645

---
An alternative is to make the mapper an observer [Gang of Four] of one or the other subsystem. That way it can be invoked by listening to events in one of them. — location: [8910](kindle://book?action=open&asin=B008OHVDFM&location=8910) ^ref-6129

---
Essentially a Mapper decouples different parts of a system. When you want to do this you have a choice between Mapper and Gateway (466). — location: [8914](kindle://book?action=open&asin=B008OHVDFM&location=8914) ^ref-32009

---
As a result you should only use a Mapper when you need to ensure that neither subsystem has a dependency on this interaction. — location: [8918](kindle://book?action=open&asin=B008OHVDFM&location=8918) ^ref-39281

---
the objects that a Mapper separates aren’t even aware of the mapper. — location: [8923](kindle://book?action=open&asin=B008OHVDFM&location=8923) ^ref-19360

---
A type that acts as the supertype for all types in its layer. — location: [8924](kindle://book?action=open&asin=B008OHVDFM&location=8924) ^ref-834

---
It’s not uncommon for all the objects in a layer to have methods you don’t want to have duplicated throughout the system. You can move all of this behavior into a common Layer Supertype. — location: [8925](kindle://book?action=open&asin=B008OHVDFM&location=8925) ^ref-26369

---
Common features, such as the storage and handling of Identity Fields (216), can go there. Similarly all Data Mappers (165) in the mapping layer can have a superclass that relies on the fact that all domain objects have a common superclass. — location: [8929](kindle://book?action=open&asin=B008OHVDFM&location=8929) ^ref-41249

---
Defines an interface in a separate package from its implementation. — location: [8941](kindle://book?action=open&asin=B008OHVDFM&location=8941) ^ref-59144

---
you might need to invoke methods that contradict the general dependency structure. If so, use Separated Interface to define an interface in one package but implement it in another. This way a client that needs the dependency to the interface can be completely unaware of the implementation. The Separated Interface provides a good plug point for Gateway (466). — location: [8946](kindle://book?action=open&asin=B008OHVDFM&location=8946) ^ref-65295

---
Essentially it takes advantage of the fact that an implementation has a dependency to its interface but not vice versa. — location: [8949](kindle://book?action=open&asin=B008OHVDFM&location=8949) ^ref-37669

---
Other packages can depend on the interface package without depending on the implementation package. — location: [8951](kindle://book?action=open&asin=B008OHVDFM&location=8951) ^ref-37667

---
You can place the interface in the client’s package (as in the sketch) or in a third package (Figure 18.1). If there’s only one client for the implementation, or all the clients are in the same package, then you might as well put the interface in with the client. A — location: [8954](kindle://book?action=open&asin=B008OHVDFM&location=8954) ^ref-15846

---
Essentially the client package indicates that it will work with any other package that implements the interface it defines. If you have multiple client packages, a third interface package is better. — location: [8957](kindle://book?action=open&asin=B008OHVDFM&location=8957) ^ref-62314

---
An abstract class can make a good interface because you can have common, but optional, implementation behavior in it. — location: [8963](kindle://book?action=open&asin=B008OHVDFM&location=8963) ^ref-3555

---
The common approach is to use a separate factory object, where again there is a Separated Interface for the factory. — location: [8965](kindle://book?action=open&asin=B008OHVDFM&location=8965) ^ref-61831

---
a simpler alternative is to let yet another package that knows both the interface and the implementation instantiate the right objects at application startup. — location: [8968](kindle://book?action=open&asin=B008OHVDFM&location=8968) ^ref-28061

---
You use Separated Interface when you need to break a dependency between two parts of the system. — location: [8971](kindle://book?action=open&asin=B008OHVDFM&location=8971) ^ref-1441

---
You have some code in one layer that needs to call code in another layer that it shouldn’t see, such as domain code calling a Data Mapper (165). — location: [8974](kindle://book?action=open&asin=B008OHVDFM&location=8974) ^ref-11595

---
I come across many developers who have separate interfaces for every class they write. I think this is excessive, especially for application development. — location: [8976](kindle://book?action=open&asin=B008OHVDFM&location=8976) ^ref-17010

---
For applications I recommend using a separate interface only if you want to break a dependency or you want to have multiple independent implementations. — location: [8979](kindle://book?action=open&asin=B008OHVDFM&location=8979) ^ref-12071

---
Registry A well-known object that other objects can use to find common objects and services. — location: [8984](kindle://book?action=open&asin=B008OHVDFM&location=8984) ^ref-55609

---
A Registry is essentially a global object, or at least it looks like one—even if it isn’t as global as it may appear. — location: [8990](kindle://book?action=open&asin=B008OHVDFM&location=8990) ^ref-18029

---
The first thing to think of is the interface, and for Registries my preferred interface is static methods. A static method on a class is easy to find anywhere in an application. — location: [8993](kindle://book?action=open&asin=B008OHVDFM&location=8993) ^ref-26277

---
Despite the encapsulation of a method, a Registry is still global data and as such is something I’m uncomfortable using. — location: [9026](kindle://book?action=open&asin=B008OHVDFM&location=9026) ^ref-10488

---
Basically, you should only use a Registry as a last resort. — location: [9028](kindle://book?action=open&asin=B008OHVDFM&location=9028) ^ref-63936

---
Value Object A small simple object, like money or a date range, whose equality isn’t based on identity. — location: [9097](kindle://book?action=open&asin=B008OHVDFM&location=9097) ^ref-33065

---
In a broad sense we like to think that Value Objects are small objects, such as a money object or a date, while reference objects are large, such as an order or a customer. — location: [9102](kindle://book?action=open&asin=B008OHVDFM&location=9102) ^ref-8804

---
The key difference between reference and value objects lies in how they deal with equality. A reference object uses identity as the basis for equality— — location: [9103](kindle://book?action=open&asin=B008OHVDFM&location=9103) ^ref-28830

---
database. A Value Object bases its notion of equality on field values within the class. Thus, two date objects may be the same if their day, month, and year values are the same. — location: [9106](kindle://book?action=open&asin=B008OHVDFM&location=9106) ^ref-7559

---
Value Objects shouldn’t be persisted as complete records. Instead use Embedded Value (268) or Serialized LOB (272). — location: [9116](kindle://book?action=open&asin=B008OHVDFM&location=9116) ^ref-3925

---
Special Case A subclass that provides special behavior for particular cases. — location: [9283](kindle://book?action=open&asin=B008OHVDFM&location=9283) ^ref-32419

---
since a variable can contain null, you may run into a runtime error by invoking a message on null, — location: [9288](kindle://book?action=open&asin=B008OHVDFM&location=9288) ^ref-37805

---
Often the right thing is the same in many contexts, so you end up writing similar code in lots of places—committing the sin of code duplication. — location: [9290](kindle://book?action=open&asin=B008OHVDFM&location=9290) ^ref-8101

---

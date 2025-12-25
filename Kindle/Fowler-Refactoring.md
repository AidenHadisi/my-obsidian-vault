---
kindle-sync:
  bookId: '21207'
  title: >-
    Refactoring: Improving the Design of Existing Code (Addison-Wesley Signature
    Series (Fowler))
  author: Martin Fowler
  asin: B07LCM8RG2
  lastAnnotatedDate: '2024-09-17'
  bookImageUrl: 'https://m.media-amazon.com/images/I/71yPDDIwcoL._SY160.jpg'
  highlightsCount: 198
---
# Refactoring
## Metadata
* Author: [Martin Fowler](https://www.amazon.comundefined)
* ASIN: B07LCM8RG2
* Reference: https://www.amazon.com/dp/B07LCM8RG2
* [Kindle link](kindle://book?action=open&asin=B07LCM8RG2)

## Highlights
When you have to add a feature to a program but the code is not structured in a convenient way, first refactor the program to make it easy to add the feature, then add the feature. — location: [471](kindle://book?action=open&asin=B07LCM8RG2&location=471) ^ref-64478

---
This being JavaScript, I can extract amountFor into a nested function of statement. This is helpful as it means I don’t have to pass data that’s inside the scope of the containing function to the newly extracted function. — location: [578](kindle://book?action=open&asin=B07LCM8RG2&location=578) ^ref-41442

---
always call the return value from a function “result”. That way I always know its role. — location: [601](kindle://book?action=open&asin=B07LCM8RG2&location=601) ^ref-26974

---
Any fool can write code that a computer can understand. Good programmers write code that humans can understand. — location: [617](kindle://book?action=open&asin=B07LCM8RG2&location=617) ^ref-48709

---
Never be afraid to change names to improve clarity. — location: [619](kindle://book?action=open&asin=B07LCM8RG2&location=619) ^ref-27848

---
When I’m breaking down a long function, I like to get rid of variables like play, because temporary variables create a lot of locally scoped names that complicate extractions. The refactoring I will use here is Replace Temp with Query (178). — location: [626](kindle://book?action=open&asin=B07LCM8RG2&location=626) ^ref-56840

---
Refactoring (noun): a change made to the internal structure of software to make it easier to understand and cheaper to modify without changing its observable behavior. — location: [1422](kindle://book?action=open&asin=B07LCM8RG2&location=1422) ^ref-20986

---
Refactoring (verb): to restructure software by applying a series of refactorings without changing its observable behavior. — location: [1428](kindle://book?action=open&asin=B07LCM8RG2&location=1428) ^ref-55871

---
divide my time between two distinct activities: adding functionality and refactoring. — location: [1453](kindle://book?action=open&asin=B07LCM8RG2&location=1453) ^ref-46436

---
start by trying to add a new capability, then I realize this would be much easier if the code were structured differently. So I swap hats and refactor for a while. — location: [1457](kindle://book?action=open&asin=B07LCM8RG2&location=1457) ^ref-1061

---
Who cares if the computer takes a few more cycles to compile something? Yet it does matter if it takes a programmer a week to make a change that would have taken only an hour with proper understanding of my code. — location: [1479](kindle://book?action=open&asin=B07LCM8RG2&location=1479) ^ref-50495

---
Help in understanding the code also means help in spotting bugs. — location: [1489](kindle://book?action=open&asin=B07LCM8RG2&location=1489) ^ref-14531

---
Software with a good internal design allows me to easily find how and where I need to make changes to add a new feature. Good modularity allows me to only have to understand a small subset of the code base to make a change. — location: [1514](kindle://book?action=open&asin=B07LCM8RG2&location=1514) ^ref-12416

---
The first time you do something, you just do it. The second time you do something similar, you wince at the duplication, but you do the duplicate thing anyway. The third time you do something similar, you refactor. — location: [1527](kindle://book?action=open&asin=B07LCM8RG2&location=1527) ^ref-27496

---
The best time to refactor is just before I need to add a new feature to the code base. As I do this, I look at the existing code and, often, see that if it were structured a little differently, my work would be much easier. — location: [1531](kindle://book?action=open&asin=B07LCM8RG2&location=1531) ^ref-28200

---
The same happens when fixing a bug. Once I’ve found the cause of the problem, I see that it would be much easier to fix should I unify the three bits of copied code causing the error into one. — location: [1543](kindle://book?action=open&asin=B07LCM8RG2&location=1543) ^ref-18028

---
Whenever I have to think to understand what the code is doing, I ask myself if I can refactor the code to make that understanding more immediately apparent. — location: [1549](kindle://book?action=open&asin=B07LCM8RG2&location=1549) ^ref-23835

---
by refactoring I move the understanding from my head into the code itself. — location: [1552](kindle://book?action=open&asin=B07LCM8RG2&location=1552) ^ref-62296

---
variation of comprehension refactoring is when I understand what the code is doing, but realize that it’s doing it badly. — location: [1561](kindle://book?action=open&asin=B07LCM8RG2&location=1561) ^ref-1649

---
I don’t put time on my plans to do refactoring; most refactoring happens while I’m doing other things. — location: [1576](kindle://book?action=open&asin=B07LCM8RG2&location=1576) ^ref-51437

---
good developers know that, often, the fastest way to add a new feature is to change the code to make it easy to add. — location: [1587](kindle://book?action=open&asin=B07LCM8RG2&location=1587) ^ref-51017

---
If I run across code that is a mess, but I don’t need to modify it, then I don’t need to refactor — location: [1640](kindle://book?action=open&asin=B07LCM8RG2&location=1640) ^ref-37211

---
Another case is when it’s easier to rewrite it than to refactor it. — location: [1642](kindle://book?action=open&asin=B07LCM8RG2&location=1642) ^ref-810

---
The whole purpose of refactoring is to make us program faster, producing more value with less effort. — location: [1653](kindle://book?action=open&asin=B07LCM8RG2&location=1653) ^ref-684

---
When renaming a function, I need to use Rename Function (124) and to retain the old declaration as a pass-through to the new one. This complicates the interface—but it is the price I must pay to avoid breaking my clients. — location: [1684](kindle://book?action=open&asin=B07LCM8RG2&location=1684) ^ref-14591

---
Continuous Integration (CI), also known as Trunk-Based Development. With CI, each team member integrates with mainline at least once per day. — location: [1714](kindle://book?action=open&asin=B07LCM8RG2&location=1714) ^ref-19137

---
This prevents any branches diverting too far from each — location: [1715](kindle://book?action=open&asin=B07LCM8RG2&location=1715) ^ref-14445

---
Refactoring can be a fantastic tool to help understand a legacy system. — location: [1756](kindle://book?action=open&asin=B07LCM8RG2&location=1756) ^ref-40272

---
The essence of the technique is to combine the structural changes to a database’s schema and access code with data migration scripts that can easily compose to handle large changes. — location: [1775](kindle://book?action=open&asin=B07LCM8RG2&location=1775) ^ref-27255

---
database changes often are best separated over multiple releases to production. This makes it easy to reverse any change that causes a problem in production. — location: [1786](kindle://book?action=open&asin=B07LCM8RG2&location=1786) ^ref-22415

---
To make the software easier to understand, I often make changes that will cause the program to run slower. — location: [1851](kindle://book?action=open&asin=B07LCM8RG2&location=1851) ^ref-8197

---
The second approach is the constant attention approach. Here, every programmer, all the time, does whatever she can to keep performance high. — location: [1860](kindle://book?action=open&asin=B07LCM8RG2&location=1860) ^ref-9434

---
One of the most important parts of clear code is good names, — location: [2018](kindle://book?action=open&asin=B07LCM8RG2&location=2018) ^ref-54484

---
When you can’t think of a good name for something, it’s often a sign of a deeper design malaise. — location: [2026](kindle://book?action=open&asin=B07LCM8RG2&location=2026) ^ref-62364

---
If you see the same code structure in more than one place, you can be sure that your program will be better if you find a way to unify them. — location: [2028](kindle://book?action=open&asin=B07LCM8RG2&location=2028) ^ref-21073

---
you have code that’s similar, but not quite identical, see if you can use Slide Statements (223) to arrange the code so the similar items are all together for easy extraction. — location: [2033](kindle://book?action=open&asin=B07LCM8RG2&location=2033) ^ref-29614

---
the longer a function is, the more difficult it is to understand. — location: [2042](kindle://book?action=open&asin=B07LCM8RG2&location=2042) ^ref-22462

---
whenever we feel the need to comment something, we write a function instead. — location: [2048](kindle://book?action=open&asin=B07LCM8RG2&location=2048) ^ref-42505

---
Ninety-nine percent of the time, all you have to do to shorten a function is Extract Function (106). Find parts of the function that seem to go nicely together and make a new one. — location: [2052](kindle://book?action=open&asin=B07LCM8RG2&location=2052) ^ref-56524

---
You can often use Replace Temp with Query (178) to eliminate the temps. Long lists of parameters can be slimmed down with Introduce Parameter Object (140) and Preserve Whole Object (319). — location: [2057](kindle://book?action=open&asin=B07LCM8RG2&location=2057) ^ref-50462

---
you’ve tried that and you still have too many temps and parameters, it’s time to get out the heavy artillery: Replace Function with Command (337). — location: [2062](kindle://book?action=open&asin=B07LCM8RG2&location=2062) ^ref-54833

---
How do you identify the clumps of code to extract? A good technique is to look for comments. — location: [2064](kindle://book?action=open&asin=B07LCM8RG2&location=2064) ^ref-668

---
Conditionals and loops also give signs for extractions. Use Decompose Conditional (260) to deal with conditional expressions. A — location: [2067](kindle://book?action=open&asin=B07LCM8RG2&location=2067) ^ref-36097

---
than one switch statement switching on the same condition, you should apply Replace Conditional with Polymorphism — location: [2071](kindle://book?action=open&asin=B07LCM8RG2&location=2071) ^ref-23127

---
With loops, extract the loop and the code within the loop into its own method. — location: [2073](kindle://book?action=open&asin=B07LCM8RG2&location=2073) ^ref-28561

---
don’t be afraid to use Split Loop (227) to break out the separate tasks. — location: [2074](kindle://book?action=open&asin=B07LCM8RG2&location=2074) ^ref-14788

---
If you can obtain one parameter by asking another parameter for it, you can use Replace Parameter with Query (324) to remove the second parameter. — location: [2078](kindle://book?action=open&asin=B07LCM8RG2&location=2078) ^ref-55006

---
Rather than pulling lots of data out of an existing data structure, you can use Preserve Whole Object (319) to pass the original data structure instead. — location: [2080](kindle://book?action=open&asin=B07LCM8RG2&location=2080) ^ref-7023

---
If several parameters always fit together, combine them with Introduce Parameter Object (140). If a parameter is used as a flag to dispatch different behavior, use Remove Flag Argument (314). — location: [2083](kindle://book?action=open&asin=B07LCM8RG2&location=2083) ^ref-33341

---
you can use Combine Functions into Class (144) to capture those common values as fields. — location: [2087](kindle://book?action=open&asin=B07LCM8RG2&location=2087) ^ref-34743

---
Global data is especially nasty when it’s mutable. Global data that you can guarantee never changes after the program starts is relatively safe—if you have a language that can enforce that guarantee. — location: [2100](kindle://book?action=open&asin=B07LCM8RG2&location=2100) ^ref-54773

---
You can use Encapsulate Variable (132) to ensure that all updates occur through narrow functions that can be easier to monitor and evolve. If a variable is being updated to store different things, use Split Variable (240) both to keep them separate and avoid the risky update. — location: [2111](kindle://book?action=open&asin=B07LCM8RG2&location=2111) ^ref-21931

---
Mutable data that can be calculated elsewhere is particularly pungent. — location: [2124](kindle://book?action=open&asin=B07LCM8RG2&location=2124) ^ref-50277

---
Mutable data isn’t a big problem when it’s a variable whose scope is just a couple of lines—but its risk increases as its scope grows. — location: [2127](kindle://book?action=open&asin=B07LCM8RG2&location=2127) ^ref-40954

---
If a variable contains some data with internal structure, it’s usually better to replace the entire structure rather than modify it in place, — location: [2131](kindle://book?action=open&asin=B07LCM8RG2&location=2131) ^ref-19269

---
Divergent change occurs when one module is often changed in different ways for different reasons. — location: [2136](kindle://book?action=open&asin=B07LCM8RG2&location=2136) ^ref-44886

---
If the two aspects naturally form a sequence—for example, you get data from the database and then apply your financial processing on it—then Split Phase (154) separates the two with a clear data structure between them. — location: [2143](kindle://book?action=open&asin=B07LCM8RG2&location=2143) ^ref-3624

---
Shotgun surgery is similar to divergent change but is the opposite. You whiff this when, every time you make a change, you have to make a lot of little edits to a lot of different classes. — location: [2152](kindle://book?action=open&asin=B07LCM8RG2&location=2152) ^ref-15964

---
you want to use Move Function (198) and Move Field (207) to put all the changes into a single module. — location: [2155](kindle://book?action=open&asin=B07LCM8RG2&location=2155) ^ref-32401

---
useful tactic for shotgun surgery is to use inlining refactorings, such as Inline Function (115) or Inline Class (186), to pull together poorly separated logic. — location: [2163](kindle://book?action=open&asin=B07LCM8RG2&location=2163) ^ref-37054

---
classic case of Feature Envy occurs when a function in one module spends more time communicating with functions or data inside another module than it does within its own module. — location: [2171](kindle://book?action=open&asin=B07LCM8RG2&location=2171) ^ref-46088

---
function clearly wants to be with the data, so use Move Function (198) to get it there. — location: [2173](kindle://book?action=open&asin=B07LCM8RG2&location=2173) ^ref-65167

---
fundamental rule of thumb is to put things together that change together. Data — location: [2184](kindle://book?action=open&asin=B07LCM8RG2&location=2184) ^ref-17697

---
Bunches of data that hang around together really ought to find a home together. — location: [2190](kindle://book?action=open&asin=B07LCM8RG2&location=2190) ^ref-7452

---
Use Extract Class (182) on the fields to turn the clumps into an object. — location: [2191](kindle://book?action=open&asin=B07LCM8RG2&location=2191) ^ref-58439

---
Then turn your attention to method signatures using Introduce Parameter Object (140) or Preserve Whole Object (319) to slim them down. — location: [2193](kindle://book?action=open&asin=B07LCM8RG2&location=2193) ^ref-900

---
A good test is to consider deleting one of the data values. If you did this, would the others make any sense? If they don’t, it’s a sure sign that you have an object that’s dying to be born. — location: [2198](kindle://book?action=open&asin=B07LCM8RG2&location=2198) ^ref-51109

---
You can now look for cases of feature envy, which will suggest behavior that can be moved into your new classes. — location: [2200](kindle://book?action=open&asin=B07LCM8RG2&location=2200) ^ref-26391

---
You can move out of the primitive cave into the centrally heated world of meaningful types by using Replace Primitive with Object (174). — location: [2210](kindle://book?action=open&asin=B07LCM8RG2&location=2210) ^ref-41133

---
If the primitive is a type code controlling conditional behavior, use Replace Type Code with Subclasses (362) followed by Replace Conditional with Polymorphism (272). — location: [2212](kindle://book?action=open&asin=B07LCM8RG2&location=2212) ^ref-2672

---
Groups of primitives that commonly appear together are data clumps and should be civilized with Extract Class (182) and Introduce Parameter Object (140). — location: [2216](kindle://book?action=open&asin=B07LCM8RG2&location=2216) ^ref-361

---
They’ll argue that any switch statement you see is begging for Replace Conditional with Polymorphism (272). — location: [2221](kindle://book?action=open&asin=B07LCM8RG2&location=2221) ^ref-55059

---
These days, however, first-class functions are widely supported, so we can use Replace Loop with Pipeline (231) to retire those anachronisms. — location: [2233](kindle://book?action=open&asin=B07LCM8RG2&location=2233) ^ref-1666

---
sometimes the structure isn’t needed. It may be a function that’s named the same as its body code reads, or a class that is essentially one simple function. — location: [2239](kindle://book?action=open&asin=B07LCM8RG2&location=2239) ^ref-40263

---
Either way, such program elements need to die with dignity. Usually this means using Inline Function (115) or Inline Class (186). With inheritance, you can use Collapse Hierarchy (380). — location: [2241](kindle://book?action=open&asin=B07LCM8RG2&location=2241) ^ref-3382

---
If you have abstract classes that aren’t doing much, use Collapse Hierarchy — location: [2250](kindle://book?action=open&asin=B07LCM8RG2&location=2250) ^ref-10398

---
Unnecessary delegation can be removed with Inline Function (115) and Inline Class (186). — location: [2252](kindle://book?action=open&asin=B07LCM8RG2&location=2252) ^ref-37828

---
Functions with unused parameters should be subject to Change Function Declaration (124) to remove those parameters. — location: [2255](kindle://book?action=open&asin=B07LCM8RG2&location=2255) ^ref-12480

---
Speculative generality can be spotted when the only users of a function or class are test cases. If you find such an animal, delete — location: [2259](kindle://book?action=open&asin=B07LCM8RG2&location=2259) ^ref-10483

---
Sometimes you see a class in which a field is set only in certain circumstances. Such code is difficult to understand, because you expect an object to need all of its fields. — location: [2262](kindle://book?action=open&asin=B07LCM8RG2&location=2262) ^ref-63055

---
You may also be able to eliminate conditional code by using Introduce Special Case (289) to create an alternative class for when the variables aren’t valid. — location: [2267](kindle://book?action=open&asin=B07LCM8RG2&location=2267) ^ref-57906

---
Navigating this way means the client is coupled to the structure of the navigation. Any change to the intermediate relationships causes the client to have to change. — location: [2272](kindle://book?action=open&asin=B07LCM8RG2&location=2272) ^ref-9575

---
The move to use here is Hide Delegate (189). You can do this at various points in the chain. — location: [2274](kindle://book?action=open&asin=B07LCM8RG2&location=2274) ^ref-47323

---
principle, you can do this to every object in the chain, but doing this often turns every intermediate object into a middle man. Often, a better alternative is to see what the resulting object is used for. See — location: [2275](kindle://book?action=open&asin=B07LCM8RG2&location=2275) ^ref-26131

---
this can go too far. You look at a class’s interface and find half the methods are delegating to this other class. — location: [2286](kindle://book?action=open&asin=B07LCM8RG2&location=2286) ^ref-24753

---
it is time to use Remove Middle Man (192) and talk to the object that really knows what’s going on. — location: [2286](kindle://book?action=open&asin=B07LCM8RG2&location=2286) ^ref-28777

---
If only a few methods aren’t doing much, use Inline Function (115) to inline them into the caller. If there is additional behavior, you can use Replace Superclass with Delegate (399) or Replace Subclass with Delegate (381) to fold the middle man into the real object. — location: [2288](kindle://book?action=open&asin=B07LCM8RG2&location=2288) ^ref-51175

---
make things work, some trade has to occur, but we need to reduce it to a minimum and keep it all above board. — location: [2296](kindle://book?action=open&asin=B07LCM8RG2&location=2296) ^ref-35735

---
Modules that whisper to each other by the coffee machine need to be separated by using Move Function (198) and Move Field (207) to reduce the need to chat. — location: [2297](kindle://book?action=open&asin=B07LCM8RG2&location=2297) ^ref-46882

---
use Hide Delegate (189) to make another module act as an intermediary. — location: [2301](kindle://book?action=open&asin=B07LCM8RG2&location=2301) ^ref-6811

---
Inheritance can often lead to collusion. Subclasses are always going to know more about their parents than their parents would like them to know. If it’s time to leave home, apply Replace Subclass with Delegate (381) or Replace Superclass with Delegate — location: [2303](kindle://book?action=open&asin=B07LCM8RG2&location=2303) ^ref-30258

---
common prefixes or suffixes for some subset of the variables in a class suggest the opportunity for a component. — location: [2311](kindle://book?action=open&asin=B07LCM8RG2&location=2311) ^ref-37662

---
the component makes sense with inheritance, you’ll find Extract Superclass (375) or Replace Type Code with Subclasses (362) (which essentially is extracting a subclass) are often easier. — location: [2312](kindle://book?action=open&asin=B07LCM8RG2&location=2312) ^ref-26647

---
The clients of such a class are often the best clue for splitting up the class. Look at whether clients use a subset of the features of the class. Each subset is a possible separate class. — location: [2320](kindle://book?action=open&asin=B07LCM8RG2&location=2320) ^ref-3381

---
One of the great benefits of using classes is the support for substitution, allowing one class to swap in for another in times of need. But this only works if their interfaces are the same. Use Change Function Declaration (124) to make functions match up. — location: [2327](kindle://book?action=open&asin=B07LCM8RG2&location=2327) ^ref-61884

---
classes that have fields, getting and setting methods for the fields, and nothing else. Such classes are dumb data holders and are often being manipulated in far too much detail by other classes. — location: [2334](kindle://book?action=open&asin=B07LCM8RG2&location=2334) ^ref-39223

---
Look for where these getting and setting methods are used by other classes. Try to use Move Function (198) to move behavior into the data class. — location: [2339](kindle://book?action=open&asin=B07LCM8RG2&location=2339) ^ref-25086

---
Data classes are often a sign of behavior in the wrong place, which means you can make big progress by moving it from the client into the data class itself. — location: [2343](kindle://book?action=open&asin=B07LCM8RG2&location=2343) ^ref-31608

---
there are exceptions, and one of the best exceptions is a record that’s being used as a result record from a distinct function invocation. A good example of this is the intermediate data structure after you’ve applied Split Phase (154). A key characteristic of such a result record is that it’s immutable (at least in practice). — location: [2344](kindle://book?action=open&asin=B07LCM8RG2&location=2344) ^ref-29950

---
The traditional story is that this means the hierarchy is wrong. You need to create a new sibling class and use Push Down Method (359) and Push Down Field (361) to push all the unused code to the sibling. That way the parent holds only what is common. — location: [2351](kindle://book?action=open&asin=B07LCM8RG2&location=2351) ^ref-16474

---
In this case, however, don’t fiddle with the hierarchy; you want to gut it by applying Replace Subclass with Delegate (381) or Replace Superclass with Delegate (399). — location: [2361](kindle://book?action=open&asin=B07LCM8RG2&location=2361) ^ref-14513

---
comments are often used as a deodorant. It’s surprising how often you look at thickly commented code and notice that the comments are there because the code is bad. — location: [2367](kindle://book?action=open&asin=B07LCM8RG2&location=2367) ^ref-44238

---
When you feel the need to write a comment, first try to refactor the code so that any comment becomes superfluous. — location: [2376](kindle://book?action=open&asin=B07LCM8RG2&location=2376) ^ref-51203

---
look at a fragment of code, understand what it is doing, then extract it into its own function named after its purpose. — location: [2795](kindle://book?action=open&asin=B07LCM8RG2&location=2795) ^ref-30326

---
If you have to spend effort looking at a fragment of code and figuring out what it’s doing, then you should extract it into a function and name the function after the “what.” — location: [2799](kindle://book?action=open&asin=B07LCM8RG2&location=2799) ^ref-22855

---
If I see an assignment to a parameter, I immediately use Split Variable (240), which turns it into a temp. — location: [2908](kindle://book?action=open&asin=B07LCM8RG2&location=2908) ^ref-41517

---
sometimes, I do come across a function in which the body is as clear as the name. Or, I refactor the body of the code into something that is just as clear as the name. When this happens, I get rid of the function. — location: [2973](kindle://book?action=open&asin=B07LCM8RG2&location=2973) ^ref-14448

---
Inline Function when I see code that’s using too much indirection—when it seems that every function does simple delegation to another function, and I get lost in all the delegation. — location: [2976](kindle://book?action=open&asin=B07LCM8RG2&location=2976) ^ref-42606

---
Expressions can become very complex and hard to read. In such situations, local variables may help break the expression down into something more manageable. — location: [3041](kindle://book?action=open&asin=B07LCM8RG2&location=3041) ^ref-60200

---
But sometimes, the name doesn’t really communicate more than the expression itself. At other times, you may find that a variable gets in the way of refactoring the neighboring code. In these cases, it can be useful to inline the variable. — location: [3126](kindle://book?action=open&asin=B07LCM8RG2&location=3126) ^ref-57210

---
good name allows me to understand what the function does when I see it called, without seeing the code that defines its implementation. — location: [3145](kindle://book?action=open&asin=B07LCM8RG2&location=3145) ^ref-44516

---
Similar logic applies to a function’s parameters. The parameters of a function dictate how a function fits in with the rest of its world. Parameters set the context in which I can use a function. If — location: [3151](kindle://book?action=open&asin=B07LCM8RG2&location=3151) ^ref-35636

---
if I want to move widely accessed data, often the best approach is to first encapsulate it by routing all its access through functions. That — location: [3326](kindle://book?action=open&asin=B07LCM8RG2&location=3326) ^ref-22679

---
Encapsulating data is valuable for other things too. It provides a clear point to monitor changes and use of the data; I can easily add validation or consequential logic on the updates. — location: [3328](kindle://book?action=open&asin=B07LCM8RG2&location=3328) ^ref-41973

---
make all mutable data encapsulated — location: [3329](kindle://book?action=open&asin=B07LCM8RG2&location=3329) ^ref-62176

---
The greater the scope of the data, the more important it is to encapsulate. — location: [3330](kindle://book?action=open&asin=B07LCM8RG2&location=3330) ^ref-56142

---
Whenever I see a public field, I consider using Encapsulate Variable (in that case often called Encapsulate Field) — location: [3333](kindle://book?action=open&asin=B07LCM8RG2&location=3333) ^ref-23987

---
Keeping data encapsulated is much less important for immutable data. When the data doesn’t change, I don’t need a place to put in validation or other logic hooks before updates. — location: [3337](kindle://book?action=open&asin=B07LCM8RG2&location=3337) ^ref-36115

---
Grouping data into a structure is valuable because it makes explicit the relationship between the data items. — location: [3487](kindle://book?action=open&asin=B07LCM8RG2&location=3487) ^ref-20465

---
An alternative to Combine Functions into Transform is Combine Functions into Class (144) that moves the logic into methods on a class formed from the source data. Either of these refactorings are helpful, — location: [3722](kindle://book?action=open&asin=B07LCM8RG2&location=3722) ^ref-42484

---
Using a class is much better if the source data gets updated within the code. Using a transform stores derived data in the new record, so if the source data changes, I will run into inconsistencies. — location: [3725](kindle://book?action=open&asin=B07LCM8RG2&location=3725) ^ref-53540

---
I can deal with this repetition by using Extract Function (106) on these calculations, but such functions often end up scattered around the program making it hard for future developers to realize they are there. — location: [3755](kindle://book?action=open&asin=B07LCM8RG2&location=3755) ^ref-24968

---
way of dealing with this is to move all of these derivations into a transformation step that takes the raw reading and emits a reading enriched with all the common derived results. — location: [3763](kindle://book?action=open&asin=B07LCM8RG2&location=3763) ^ref-54149

---
When I’m applying a transformation that produces essentially the same thing but with additional information, I like to name it using “enrich”. If it were producing something I felt was different, I would name it using “transform”. — location: [3769](kindle://book?action=open&asin=B07LCM8RG2&location=3769) ^ref-61572

---
When I run into code that’s dealing with two different things, I look for a way to split it into separate modules. — location: [3844](kindle://book?action=open&asin=B07LCM8RG2&location=3844) ^ref-49730

---
One of the neatest ways to do a split like this is to divide the behavior into two sequential phases. — location: [3846](kindle://book?action=open&asin=B07LCM8RG2&location=3846) ^ref-40186

---
Perhaps the most important criteria to be used in decomposing modules is to identify secrets that modules should hide from the rest of the system — location: [3961](kindle://book?action=open&asin=B07LCM8RG2&location=3961) ^ref-51062

---
Classes and modules are the largest forms of encapsulation, but functions also encapsulate their implementation. — location: [3980](kindle://book?action=open&asin=B07LCM8RG2&location=3980) ^ref-13221

---
favor objects over records for mutable data. — location: [3992](kindle://book?action=open&asin=B07LCM8RG2&location=3992) ^ref-35711

---
The user of the object doesn’t need to know or care which is stored and which is calculated. — location: [3993](kindle://book?action=open&asin=B07LCM8RG2&location=3993) ^ref-10995

---
If I have an immutable value, I can just have all three values in my record, using an enrichment step if necessary. — location: [3996](kindle://book?action=open&asin=B07LCM8RG2&location=3996) ^ref-54899

---
I gave the getter a name deliberately chosen to be both ugly and easy to search for. This is because I intend its life to be short. — location: [4040](kindle://book?action=open&asin=B07LCM8RG2&location=4040) ^ref-27096

---
encapsulating any mutable data in my programs. This makes it easier to see when and how data structures are modified, which then makes it easier to change those data structures — location: [4201](kindle://book?action=open&asin=B07LCM8RG2&location=4201) ^ref-4633

---
Access to a collection variable may be encapsulated, but if the getter returns the collection itself, then that collection’s membership can be altered without the enclosing class being able to intervene. — location: [4203](kindle://book?action=open&asin=B07LCM8RG2&location=4203) ^ref-35112

---
To avoid this, I provide collection modifier methods—usually add and remove—on the class itself. — location: [4205](kindle://book?action=open&asin=B07LCM8RG2&location=4205) ^ref-20544

---
ensure that the getter for the collection does not return the raw collection, so that clients cannot accidentally change it. — location: [4209](kindle://book?action=open&asin=B07LCM8RG2&location=4209) ^ref-5174

---
One way to prevent modification of the underlying collection is by never returning a collection value. In this approach, any use of a collection field is done with specific methods on the owning class, — location: [4210](kindle://book?action=open&asin=B07LCM8RG2&location=4210) ^ref-34136

---
Probably the most common approach is to provide a getting method for the collection, but make it return a copy of the underlying collection. — location: [4218](kindle://book?action=open&asin=B07LCM8RG2&location=4218) ^ref-59112

---
This violates encapsulating because the person class has no ability to take control when the list is updated in this way. While the reference to the field is encapsulated, the content of the field is not. — location: [4258](kindle://book?action=open&asin=B07LCM8RG2&location=4258) ^ref-64240

---
Every time the client wants to use a new feature of the delegate, I have to add a simple delegating method to the server. After adding features for a while, I get irritated with all this forwarding. The server class is just a middle man (Middle Man (81)), and perhaps it’s time for the client to call the delegate directly. — location: [4673](kindle://book?action=open&asin=B07LCM8RG2&location=4673) ^ref-38611

---
Sometimes, when I want to change the algorithm to work slightly differently, it’s easier to start by replacing it with something that would make my change more straightforward to make. When I have — location: [4735](kindle://book?action=open&asin=B07LCM8RG2&location=4735) ^ref-13406

---
need to ensure that related software elements are grouped together and the links between them are easy to find and understand. — location: [4768](kindle://book?action=open&asin=B07LCM8RG2&location=4768) ^ref-43741

---
One of the most straightforward reasons to move a function is when it references elements in other contexts more than the one it currently resides in. — location: [4773](kindle://book?action=open&asin=B07LCM8RG2&location=4773) ^ref-26143

---
Similarly, I may move a function because of where its callers live, or where I need to call it from in my next enhancement. — location: [4775](kindle://book?action=open&asin=B07LCM8RG2&location=4775) ^ref-16983

---
Many other variables are used to hold the result of a long-winded bit of code for easy reference later. These kinds of variables should be set only once. — location: [5569](kindle://book?action=open&asin=B07LCM8RG2&location=5569) ^ref-43164

---
Any variable with more than one responsibility should be replaced with multiple variables, one for each responsibility. Using a variable for two different things is very confusing for the reader. — location: [5571](kindle://book?action=open&asin=B07LCM8RG2&location=5571) ^ref-47623

---
One of the biggest sources of problems in software is mutable data. — location: [5723](kindle://book?action=open&asin=B07LCM8RG2&location=5723) ^ref-23234

---
One way I can make a big impact is by removing any variables that I could just as easily calculate. — location: [5726](kindle://book?action=open&asin=B07LCM8RG2&location=5726) ^ref-57517

---
When I nest an object, or data structure, within another I can treat the inner object as a reference or as a value. The difference is most obviously visible in how I handle updates of the inner object’s properties. If I treat it as a reference, I’ll update the inner object’s property keeping the same inner object. If I treat it as a value, I will replace the entire inner object with a new one that has the desired property. — location: [5812](kindle://book?action=open&asin=B07LCM8RG2&location=5812) ^ref-24263

---
If I treat a field as a value, I can change the class of the inner object to make it a Value Object — location: [5815](kindle://book?action=open&asin=B07LCM8RG2&location=5815) ^ref-9841

---
Value objects are especially useful in distributed and concurrent systems. — location: [5819](kindle://book?action=open&asin=B07LCM8RG2&location=5819) ^ref-6000

---
This also suggests when I shouldn’t do this refactoring. If I want to share an object between several objects so that any change to the shared object is visible to all its collaborators, then I need the shared object to be a reference. — location: [5819](kindle://book?action=open&asin=B07LCM8RG2&location=5819) ^ref-27186

---
The biggest difficulty in having physical copies of the same logical data occurs when I need to update the shared data. I then have to find all the copies and update them all. — location: [5896](kindle://book?action=open&asin=B07LCM8RG2&location=5896) ^ref-26929

---
In this case, it’s often worthwhile to change the copied data into a single reference. — location: [5898](kindle://book?action=open&asin=B07LCM8RG2&location=5898) ^ref-31741

---
problem usually lies in the fact that the code, both in the condition checks and in the actions, tells me what happens but can easily obscure why it happens. — location: [5965](kindle://book?action=open&asin=B07LCM8RG2&location=5965) ^ref-284

---
Apply Extract Function (106) on the condition and each leg of the conditional. — location: [5973](kindle://book?action=open&asin=B07LCM8RG2&location=5973) ^ref-4547

---
series of conditional checks where each check is different yet the resulting action is the same. — location: [6010](kindle://book?action=open&asin=B07LCM8RG2&location=6010) ^ref-32132

---
use and and or operators to consolidate them into a single conditional check with a single result. — location: [6011](kindle://book?action=open&asin=B07LCM8RG2&location=6011) ^ref-9560

---
If both are part of normal behavior, I use a condition with an if and an else leg. If the condition is an unusual condition, I check the condition and return if it’s true. This kind of check is often called a guard clause. — location: [6073](kindle://book?action=open&asin=B07LCM8RG2&location=6073) ^ref-34743

---
Complex conditional logic is one of the hardest things to reason about in programming, — location: [6170](kindle://book?action=open&asin=B07LCM8RG2&location=6170) ^ref-32050

---
A common case for this is where I can form a set of types, each handling the conditional logic differently. — location: [6174](kindle://book?action=open&asin=B07LCM8RG2&location=6174) ^ref-55735

---
This is made most obvious when there are several functions that have a switch statement on a type code. — location: [6175](kindle://book?action=open&asin=B07LCM8RG2&location=6175) ^ref-4110

---
In that case, I remove the duplication of the common switch logic by creating classes for each case and using polymorphism to bring out the type-specific behavior. — location: [6176](kindle://book?action=open&asin=B07LCM8RG2&location=6176) ^ref-52790

---
A common case of duplicated code is when many users of a data structure check a specific value, and then most of them do the same thing. — location: [6516](kindle://book?action=open&asin=B07LCM8RG2&location=6516) ^ref-32723

---
If I find many parts of the code base having the same reaction to a particular value, I want to bring that reaction into a single place. — location: [6517](kindle://book?action=open&asin=B07LCM8RG2&location=6517) ^ref-49887

---
ways. If all I’m doing with the object is reading data, I can supply a literal object with all the values I need filled in. — location: [6520](kindle://book?action=open&asin=B07LCM8RG2&location=6520) ^ref-4422

---
If I need more behavior than simple values, I can create a special object with methods for all the common behavior. — location: [6521](kindle://book?action=open&asin=B07LCM8RG2&location=6521) ^ref-22449

---
It is a good idea to clearly signal the difference between functions with side effects and those without. — location: [6931](kindle://book?action=open&asin=B07LCM8RG2&location=6931) ^ref-48081

---
A good rule to follow is that any function that returns a value should not have observable side effects—the command-query separation [mf-cqs]. — location: [6932](kindle://book?action=open&asin=B07LCM8RG2&location=6932) ^ref-65173

---
If I come across a method that returns a value but also has side effects, I always try to separate the query from the modifier. — location: [6934](kindle://book?action=open&asin=B07LCM8RG2&location=6934) ^ref-25882

---
If I see two functions that carry out very similar logic with different literal values, I can remove the duplication by using a single function with parameters for the different values. — location: [6990](kindle://book?action=open&asin=B07LCM8RG2&location=6990) ^ref-55540

---
argument that the — location: [7061](kindle://book?action=open&asin=B07LCM8RG2&location=7061) ^ref-63131

---
dislike flag arguments because they complicate the process of understanding what function calls are available and how to call them. — location: [7074](kindle://book?action=open&asin=B07LCM8RG2&location=7074) ^ref-27906

---
If I see code that derives a couple of values from a record and then passes these values into a function, I like to replace those values with the whole record itself, letting the function body derive the values it needs. — location: [7163](kindle://book?action=open&asin=B07LCM8RG2&location=7163) ^ref-560

---
Pulling several values from an object to do some logic on them alone is a smell (Feature Envy (77)), and usually a signal that this logic should be moved into the whole itself. — location: [7169](kindle://book?action=open&asin=B07LCM8RG2&location=7169) ^ref-32227

---
If a call passes in a value that the function can just as easily determine for itself, that’s a form of duplication— — location: [7290](kindle://book?action=open&asin=B07LCM8RG2&location=7290) ^ref-15482

---
Providing a setting method indicates that a field may be changed. If I don’t want that field to change once the object is created, I don’t provide a setting method — location: [7442](kindle://book?action=open&asin=B07LCM8RG2&location=7442) ^ref-48687

---
But there are times when it’s useful to encapsulate a function into its own object, which I refer to as a “command object” or simply a command. — location: [7546](kindle://book?action=open&asin=B07LCM8RG2&location=7546) ^ref-4078

---
Commands can have complimentary operations, such as undo. — location: [7549](kindle://book?action=open&asin=B07LCM8RG2&location=7549) ^ref-65404

---
can build in customizations using inheritance and hooks. — location: [7550](kindle://book?action=open&asin=B07LCM8RG2&location=7550) ^ref-42575

---
So, given the choice between a first-class function and a command, I’ll pick the function 95% of the time. — location: [7554](kindle://book?action=open&asin=B07LCM8RG2&location=7554) ^ref-29957

---
One of these cases is breaking up a complex function so I can better understand and modify it. — location: [7573](kindle://book?action=open&asin=B07LCM8RG2&location=7573) ^ref-16965

---
Command objects provide a powerful mechanism for handling complex computations. They can easily be broken down into separate methods sharing common state through the fields; — location: [7673](kindle://book?action=open&asin=B07LCM8RG2&location=7673) ^ref-42853

---
can be invoked via different methods for different effects; — location: [7674](kindle://book?action=open&asin=B07LCM8RG2&location=7674) ^ref-40451

---
Whenever there is duplication, there is risk that an alteration to one copy will not be made to the other. Usually, it is difficult to find the duplicates. — location: [7791](kindle://book?action=open&asin=B07LCM8RG2&location=7791) ^ref-64418

---
The easiest case of using Pull Up Method is when the methods have the same body, implying there’s been a copy and paste. — location: [7792](kindle://book?action=open&asin=B07LCM8RG2&location=7792) ^ref-6689

---
subclasses are developed independently, or combined through refactoring, I often find that they duplicate features. In particular, certain fields can be duplicates. Such fields sometimes have similar names—but not always. — location: [7846](kindle://book?action=open&asin=B07LCM8RG2&location=7846) ^ref-31837

---
Motivation If a method is only relevant to one subclass (or a small proportion of subclasses), removing it from the superclass and putting it only on the subclass(es) makes that clearer. — location: [7938](kindle://book?action=open&asin=B07LCM8RG2&location=7938) ^ref-916

---
Most of the time, such a type code is all I need. But there are a couple of situations where I could do with something more, and that something more are subclasses. There are two things that are particularly enticing about subclasses. First, they allow me to use polymorphism to handle conditional logic. I find this most helpful when I have several functions that invoke different behavior depending on the value of the type code. With subclasses, I can apply Replace Conditional with Polymorphism (272) to these functions. — location: [7970](kindle://book?action=open&asin=B07LCM8RG2&location=7970) ^ref-23838

---
The second case is where I have fields or methods that are only valid for particular values of a type code, such as a sales quota that’s only applicable to the “salesman” type code. — location: [7975](kindle://book?action=open&asin=B07LCM8RG2&location=7975) ^ref-48815

---
relationship more explicit. When using Replace Type Code with Subclasses, I need to consider whether to apply it directly to the class I’m looking at, or to the type code itself. Do I make engineer a subtype of employee, or should I give the employee an employee type property which can have subtypes for engineer and manager? Using direct subclassing is simpler, but I can’t use it for the job type if I need it for something else. I also can’t use direct subclasses if the type is mutable. — location: [7979](kindle://book?action=open&asin=B07LCM8RG2&location=7979) ^ref-22028

---
A subclass that does too little incurs a cost in understanding that is no longer worthwhile. When that time comes, it’s best to remove the subclass, replacing it with a field on its superclass. — location: [8134](kindle://book?action=open&asin=B07LCM8RG2&location=8134) ^ref-7083

---
If I see two classes doing similar things, I can take advantage of the basic mechanism of inheritance to pull their similarities — location: [8251](kindle://book?action=open&asin=B07LCM8RG2&location=8251) ^ref-13097

---
if I want to vary behavior of people by their age category and by their income level, I can either have subclasses for young and senior, or for well-off and poor—I can’t have both. — location: [8379](kindle://book?action=open&asin=B07LCM8RG2&location=8379) ^ref-294

---
Delegation handles both of these problems. I can delegate to many different classes for different reasons. Delegation is a regular relationship between objects— — location: [8383](kindle://book?action=open&asin=B07LCM8RG2&location=8383) ^ref-28806

---
There is a popular principle: “Favor object composition over class inheritance” (where composition is effectively the same as delegation). — location: [8386](kindle://book?action=open&asin=B07LCM8RG2&location=8386) ^ref-63752

---
While it’s good to reuse, this inheritance had a problem: All the operations of the list were present on the interface of the stack, although most of them were not applicable to a stack. — location: [8811](kindle://book?action=open&asin=B07LCM8RG2&location=8811) ^ref-5446

---
A better approach is to make the list into a field of the stack and delegate the necessary operations to it. — location: [8812](kindle://book?action=open&asin=B07LCM8RG2&location=8812) ^ref-15663

---

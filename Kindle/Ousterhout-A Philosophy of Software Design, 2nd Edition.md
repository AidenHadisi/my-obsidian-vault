---
kindle-sync:
  bookId: '14934'
  title: 'A Philosophy of Software Design, 2nd Edition'
  author: John K.  Ousterhout
  asin: B09B8LFKQL
  lastAnnotatedDate: '2023-07-01'
  bookImageUrl: 'https://m.media-amazon.com/images/I/7146AYGD0AL._SY160.jpg'
  highlightsCount: 219
---
# A Philosophy of Software Design, 2nd Edition
## Metadata
* Author: [John K.  Ousterhout](https://www.amazon.comundefined)
* ASIN: B09B8LFKQL
* ISBN: 1732102228
* Reference: https://www.amazon.com/dp/B09B8LFKQL
* [Kindle link](kindle://book?action=open&asin=B09B8LFKQL)

## Highlights
The most fundamental problem in computer science is problem decomposition: how to take a complex problem and divide it up into pieces that can be solved independently. — location: [171](kindle://book?action=open&asin=B09B8LFKQL&location=171) ^ref-56123

---
If we want to make it easier to write software, so that we can build more powerful systems more cheaply, we must find ways to make software simpler. — location: [236](kindle://book?action=open&asin=B09B8LFKQL&location=236) ^ref-37708

---
The first approach is to eliminate complexity by making code simpler and more obvious. For — location: [239](kindle://book?action=open&asin=B09B8LFKQL&location=239) ^ref-30632

---
The second approach to complexity is to encapsulate it, so that programmers can work on a system without being exposed to all of its complexity at once. This approach is called modular design. — location: [241](kindle://book?action=open&asin=B09B8LFKQL&location=241) ^ref-17957

---
The modules are designed to be relatively independent of each other, so that a programmer can work on one module without having to understand the details of other modules. — location: [243](kindle://book?action=open&asin=B09B8LFKQL&location=243) ^ref-34140

---
The problems do not become apparent until implementation is well underway. — location: [253](kindle://book?action=open&asin=B09B8LFKQL&location=253) ^ref-33834

---
Each iteration exposes problems with the existing design, which are fixed before the next set of features is designed. — location: [259](kindle://book?action=open&asin=B09B8LFKQL&location=259) ^ref-37599

---
The initial design for a system or component is almost never the best one; experience inevitably shows better ways to do things. — location: [266](kindle://book?action=open&asin=B09B8LFKQL&location=266) ^ref-60859

---
One of the best ways to improve your design skills is to learn to recognize red flags: signs that a piece of code is probably more complicated than it needs to be. — location: [284](kindle://book?action=open&asin=B09B8LFKQL&location=284) ^ref-21803

---
Complexity is anything related to the structure of a software system that makes it hard to understand and modify the system. — location: [311](kindle://book?action=open&asin=B09B8LFKQL&location=311) ^ref-35742

---
If a software system is hard to understand and modify, then it is complicated; if it is easy to understand and modify, then it is simple. — location: [314](kindle://book?action=open&asin=B09B8LFKQL&location=314) ^ref-11666

---
Complexity is determined by the activities that are most common. — location: [322](kindle://book?action=open&asin=B09B8LFKQL&location=322) ^ref-41271

---
The overall complexity of a system (C) is determined by the complexity of each part p (cp) weighted by the fraction of time developers spend working on that part (tp). Isolating complexity in a place where it will never be seen is almost as good as eliminating the complexity entirely. — location: [325](kindle://book?action=open&asin=B09B8LFKQL&location=325) ^ref-24068

---
If you write a piece of code and it seems simple to you, but other people think it is complex, then it is complex. — location: [328](kindle://book?action=open&asin=B09B8LFKQL&location=328) ^ref-63188

---
Complexity manifests itself in three general ways, — location: [332](kindle://book?action=open&asin=B09B8LFKQL&location=332) ^ref-5423

---
Change amplification: The first symptom of complexity is that a seemingly simple change requires code modifications in many different places. — location: [334](kindle://book?action=open&asin=B09B8LFKQL&location=334) ^ref-25154

---
One of the goals of good design is to reduce the amount of code that is affected by each design decision, so design changes don’t require very many code modifications. — location: [340](kindle://book?action=open&asin=B09B8LFKQL&location=340) ^ref-3438

---
Cognitive load: The second symptom of complexity is cognitive load, which refers to how much a developer needs to know in order to complete a task. — location: [341](kindle://book?action=open&asin=B09B8LFKQL&location=341) ^ref-27426

---
Sometimes an approach that requires more lines of code is actually simpler, because it reduces cognitive load. — location: [351](kindle://book?action=open&asin=B09B8LFKQL&location=351) ^ref-12308

---
Unknown unknowns: The third symptom of complexity is that it is not obvious which pieces of code must be modified to complete a task, or what information a developer must have to carry out the task successfully. — location: [356](kindle://book?action=open&asin=B09B8LFKQL&location=356) ^ref-5260

---
Of the three manifestations of complexity, unknown unknowns are the worst. — location: [363](kindle://book?action=open&asin=B09B8LFKQL&location=363) ^ref-9527

---
An unknown unknown means that there is something you need to know, but there is no way for you to find out what it is, or even whether there is an issue. You won’t find out about it until bugs appear after you make a change. — location: [364](kindle://book?action=open&asin=B09B8LFKQL&location=364) ^ref-41662

---
One of the most important goals of good design is for a system to be obvious. — location: [370](kindle://book?action=open&asin=B09B8LFKQL&location=370) ^ref-25355

---
Complexity is caused by two things: dependencies and obscurity. — location: [376](kindle://book?action=open&asin=B09B8LFKQL&location=376) ^ref-38878

---
For the purposes of this book, a dependency exists when a given piece of code cannot be understood and modified in isolation; the code relates in some way to other code, and the other code must be considered and/or modified if the given code is changed. — location: [378](kindle://book?action=open&asin=B09B8LFKQL&location=378) ^ref-19844

---
The signature of a method creates a dependency between the implementation of that method and the code that invokes it: — location: [383](kindle://book?action=open&asin=B09B8LFKQL&location=383) ^ref-53674

---
one of the goals of software design is to reduce the number of dependencies and to make the dependencies that remain as simple and obvious as possible. — location: [387](kindle://book?action=open&asin=B09B8LFKQL&location=387) ^ref-2400

---
The second cause of complexity is obscurity. Obscurity occurs when important information is not obvious. — location: [395](kindle://book?action=open&asin=B09B8LFKQL&location=395) ^ref-11473

---
A simple example is a variable name that is so generic that it doesn’t carry much useful information (e.g., time). — location: [396](kindle://book?action=open&asin=B09B8LFKQL&location=396) ^ref-31345

---
Obscurity is often associated with dependencies, where it is not obvious that a dependency exists. — location: [398](kindle://book?action=open&asin=B09B8LFKQL&location=398) ^ref-1242

---
If a system has a clean and obvious design, then it will need less documentation. — location: [403](kindle://book?action=open&asin=B09B8LFKQL&location=403) ^ref-54385

---
load. If we can find design techniques that minimize dependencies and obscurity, then we can reduce the complexity of software. — location: [407](kindle://book?action=open&asin=B09B8LFKQL&location=407) ^ref-27900

---
Complexity is incremental — location: [408](kindle://book?action=open&asin=B09B8LFKQL&location=408) ^ref-43270

---
Working Code Isn’t Enough — location: [422](kindle://book?action=open&asin=B09B8LFKQL&location=422) ^ref-37446

---
tactical programming makes it nearly impossible to produce a good system design. — location: [430](kindle://book?action=open&asin=B09B8LFKQL&location=430) ^ref-18498

---
The tactical tornado is a prolific programmer who pumps out code far faster than others but works in a totally tactical fashion. — location: [447](kindle://book?action=open&asin=B09B8LFKQL&location=447) ^ref-23982

---
In some organizations, management treats tactical tornadoes as heroes. However, tactical tornadoes leave behind a wake of destruction. — location: [449](kindle://book?action=open&asin=B09B8LFKQL&location=449) ^ref-19284

---
Typically, other engineers must clean up the messes left behind by the tactical tornado, which makes it appear that those engineers (who are the real heroes) are making slower progress than the tactical tornado. — location: [450](kindle://book?action=open&asin=B09B8LFKQL&location=450) ^ref-55767

---
The first step towards becoming a good software designer is to realize that working code isn’t enough. — location: [453](kindle://book?action=open&asin=B09B8LFKQL&location=453) ^ref-60607

---
Your primary goal must be to produce a great design, which also happens to work. This is strategic programming. — location: [457](kindle://book?action=open&asin=B09B8LFKQL&location=457) ^ref-25614

---
rather than implementing the first idea that comes to mind, try a couple of alternative designs and pick the cleanest one. — location: [461](kindle://book?action=open&asin=B09B8LFKQL&location=461) ^ref-54756

---
Other investments will be reactive. No matter how much you invest up front, there will inevitably be mistakes in your design decisions. — location: [464](kindle://book?action=open&asin=B09B8LFKQL&location=464) ^ref-49543

---
The term technical debt is often used to describe the problems caused by tactical programming. — location: [486](kindle://book?action=open&asin=B09B8LFKQL&location=486) ^ref-31997

---
Unlike financial debt, most technical debt is never fully repaid: you’ll keep paying and paying forever. — location: [488](kindle://book?action=open&asin=B09B8LFKQL&location=488) ^ref-60963

---
If you are in a company leaning in this direction, you should realize that once a code base turns to spaghetti, it is nearly impossible to fix. — location: [500](kindle://book?action=open&asin=B09B8LFKQL&location=500) ^ref-26125

---
the best engineers care deeply about good design. — location: [505](kindle://book?action=open&asin=B09B8LFKQL&location=505) ^ref-54571

---
One of the most important techniques for managing software complexity is to design systems so that developers only need to face a small fraction of the overall complexity at any given time. — location: [533](kindle://book?action=open&asin=B09B8LFKQL&location=533) ^ref-28867

---
In an ideal world, each module would be completely independent of the others: a developer could work in any of the modules without knowing anything about any of the other modules. — location: [537](kindle://book?action=open&asin=B09B8LFKQL&location=537) ^ref-46873

---
this ideal is not achievable. — location: [539](kindle://book?action=open&asin=B09B8LFKQL&location=539) ^ref-25248

---
There will be dependencies between the modules: if one module changes, other modules may need to change to match. — location: [540](kindle://book?action=open&asin=B09B8LFKQL&location=540) ^ref-18246

---
The goal of modular design is to minimize the dependencies between modules. — location: [544](kindle://book?action=open&asin=B09B8LFKQL&location=544) ^ref-46332

---
we think of each module in two parts: an interface and an implementation. — location: [545](kindle://book?action=open&asin=B09B8LFKQL&location=545) ^ref-60331

---
The interface consists of everything that a developer working in a different module must know in order to use the given module. — location: [545](kindle://book?action=open&asin=B09B8LFKQL&location=545) ^ref-59224

---
Typically, the interface describes what the module does but not how it does it. — location: [546](kindle://book?action=open&asin=B09B8LFKQL&location=546) ^ref-39693

---
A developer should not need to understand the implementations of modules other than the one he or she is working in. — location: [549](kindle://book?action=open&asin=B09B8LFKQL&location=549) ^ref-4848

---
For the purposes of this book, a module is any unit of code that has an interface and an implementation. — location: [553](kindle://book?action=open&asin=B09B8LFKQL&location=553) ^ref-39344

---
The best modules are those whose interfaces are much simpler than their implementations. — location: [558](kindle://book?action=open&asin=B09B8LFKQL&location=558) ^ref-30813

---
First, a simple interface minimizes the complexity that a module imposes on the rest of the system. Second, if a module is modified in a way that does not change its interface, then no other module will be affected by the modification. — location: [559](kindle://book?action=open&asin=B09B8LFKQL&location=559) ^ref-49807

---
The informal parts of an interface include its high-level behavior, such as the fact that a function deletes the file named by one of its arguments. — location: [569](kindle://book?action=open&asin=B09B8LFKQL&location=569) ^ref-6642

---
If there are constraints on the usage of a class (perhaps one method must be called before another), these are also part of the class’s interface. — location: [570](kindle://book?action=open&asin=B09B8LFKQL&location=570) ^ref-59752

---
if a developer needs to know a particular piece of information in order to use a module, then that information is part of the module’s interface. — location: [571](kindle://book?action=open&asin=B09B8LFKQL&location=571) ^ref-11982

---
The informal aspects of an interface can only be described using comments, and the programming language cannot ensure that the description is complete or accurate1. — location: [572](kindle://book?action=open&asin=B09B8LFKQL&location=572) ^ref-45560

---
An abstraction is a simplified view of an entity, which omits unimportant details. — location: [578](kindle://book?action=open&asin=B09B8LFKQL&location=578) ^ref-59302

---
In modular programming, each module provides an abstraction in the form of its interface. — location: [579](kindle://book?action=open&asin=B09B8LFKQL&location=579) ^ref-43543

---
An abstraction can go wrong in two ways. First, it can include details that are not really important; when this happens, it makes the abstraction more complicated than necessary, which increases the cognitive load on developers using the abstraction. The second error is when an abstraction omits details that really are important. This results in obscurity: developers looking only at the abstraction will not have all the information they need to use the abstraction correctly. An abstraction that omits important details is a false abstraction: it might appear simple, but in reality it isn’t. — location: [583](kindle://book?action=open&asin=B09B8LFKQL&location=583) ^ref-62810

---
The best modules are those that provide powerful functionality yet have simple interfaces. — location: [602](kindle://book?action=open&asin=B09B8LFKQL&location=602) ^ref-862

---
A deep module is a good abstraction because only a small fraction of its internal complexity is visible to its users. — location: [607](kindle://book?action=open&asin=B09B8LFKQL&location=607) ^ref-11847

---
The best modules are those with the greatest benefit and the least cost. — location: [610](kindle://book?action=open&asin=B09B8LFKQL&location=610) ^ref-40074

---
On the other hand, a shallow module is one whose interface is relatively complex in comparison to the functionality that it provides. — location: [641](kindle://book?action=open&asin=B09B8LFKQL&location=641) ^ref-1962

---
Shallow classes like linked lists are sometimes unavoidable and they can still be useful, but they don’t provide much leverage against complexity. — location: [644](kindle://book?action=open&asin=B09B8LFKQL&location=644) ^ref-22138

---
shallow module is one whose interface is complicated relative to the functionality it provides. Shallow modules don’t help much in the battle against complexity, because the benefit they provide (not having to learn about how they work internally) is negated by the cost of learning and using their interfaces. Small modules tend to be shallow. — location: [657](kindle://book?action=open&asin=B09B8LFKQL&location=657) ^ref-7534

---
interfaces should be designed to make the common case as simple as possible — location: [690](kindle://book?action=open&asin=B09B8LFKQL&location=690) ^ref-14546

---
Almost every user of file I/O will want buffering, so it should be provided by default. For those few situations where buffering is not desirable, the library can provide a mechanism to disable it. — location: [691](kindle://book?action=open&asin=B09B8LFKQL&location=691) ^ref-13347

---
The basic idea is that each module should encapsulate a few pieces of knowledge, which represent design decisions. — location: [714](kindle://book?action=open&asin=B09B8LFKQL&location=714) ^ref-1817

---
Information hiding reduces complexity in two ways. First, it simplifies the interface to a module. — location: [722](kindle://book?action=open&asin=B09B8LFKQL&location=722) ^ref-53673

---
Second, information hiding makes it easier to evolve the system. If a piece of information is hidden, there are no dependencies on that information — location: [725](kindle://book?action=open&asin=B09B8LFKQL&location=725) ^ref-62003

---
When designing a new module, you should think carefully about what information can be hidden in that module. — location: [729](kindle://book?action=open&asin=B09B8LFKQL&location=729) ^ref-51957

---
The best form of information hiding is when information is totally hidden within a module, so that it is irrelevant and invisible to users of the module. However, partial information hiding also has value. For example, if a particular feature or piece of information is only needed by a few of a class’s users, and it is accessed through separate methods so that it isn’t visible in the most common use cases, then that information is mostly hidden. — location: [734](kindle://book?action=open&asin=B09B8LFKQL&location=734) ^ref-60688

---
The opposite of information hiding is information leakage. Information leakage occurs when a design decision is reflected in multiple modules. — location: [739](kindle://book?action=open&asin=B09B8LFKQL&location=739) ^ref-33407

---
a piece of information is reflected in the interface for a module, then by definition it has been leaked; thus, simpler interfaces tend to correlate with better information hiding. — location: [741](kindle://book?action=open&asin=B09B8LFKQL&location=741) ^ref-16960

---
If you encounter information leakage between classes, ask yourself “How can I reorganize these classes so that this particular piece of knowledge only affects a single class?” If — location: [747](kindle://book?action=open&asin=B09B8LFKQL&location=747) ^ref-24757

---
In temporal decomposition, the structure of a system corresponds to the time order in which operations will occur. — location: [755](kindle://book?action=open&asin=B09B8LFKQL&location=755) ^ref-36877

---
temporal decomposition often results in information leakage. — location: [761](kindle://book?action=open&asin=B09B8LFKQL&location=761) ^ref-21339

---
Information leakage occurs when the same knowledge is used in multiple places, such as two different classes that both understand the format of a particular type of file. — location: [764](kindle://book?action=open&asin=B09B8LFKQL&location=764) ^ref-51491

---
When designing modules, focus on the knowledge that’s needed to perform each task, not the order in which tasks occur. — location: [767](kindle://book?action=open&asin=B09B8LFKQL&location=767) ^ref-41715

---
In temporal decomposition, execution order is reflected in the code structure: operations that happen at different times are in different methods or classes. If the same knowledge is used at different points in execution, it gets encoded in multiple places, resulting in information leakage. — location: [778](kindle://book?action=open&asin=B09B8LFKQL&location=778) ^ref-34172

---
Because the classes shared so much information, it would have been better to merge them into a single class that handles both request reading and parsing. — location: [796](kindle://book?action=open&asin=B09B8LFKQL&location=796) ^ref-6604

---
in software design: information hiding can often be improved by making a class slightly larger. — location: [799](kindle://book?action=open&asin=B09B8LFKQL&location=799) ^ref-40785

---
A second reason for increasing the size of a class is to raise the level of the interface; for example, rather than having separate methods for each of three steps of a computation, have a single method that performs the entire computation. — location: [801](kindle://book?action=open&asin=B09B8LFKQL&location=801) ^ref-9707

---
Rather than returning a single parameter, the method returns a reference to the Map used internally to store all of the parameters. This method is shallow, and it exposes the internal representation used by the HTTPRequest — location: [828](kindle://book?action=open&asin=B09B8LFKQL&location=828) ^ref-26630

---
it’s important to avoid exposing internal data structures as much as possible. — location: [833](kindle://book?action=open&asin=B09B8LFKQL&location=833) ^ref-54346

---
Here is a better interface for retrieving parameter values: public String getParameter(String name) { ... } public int getIntParameter(String name) { ... } — location: [838](kindle://book?action=open&asin=B09B8LFKQL&location=838) ^ref-24676

---
Defaults illustrate the principle that interfaces should be designed to make the common case as simple as possible. — location: [856](kindle://book?action=open&asin=B09B8LFKQL&location=856) ^ref-63497

---
Whenever possible, classes should “do the right thing” without being explicitly asked. Defaults are an example of this. — location: [859](kindle://book?action=open&asin=B09B8LFKQL&location=859) ^ref-33698

---
If the API for a commonly used feature forces users to learn about other features that are rarely used, this increases the cognitive load on users who don’t need the rarely used features. — location: [865](kindle://book?action=open&asin=B09B8LFKQL&location=865) ^ref-35762

---
if you can reduce the number of places where a variable is used, you will eliminate dependencies within the class and reduce its complexity. — location: [871](kindle://book?action=open&asin=B09B8LFKQL&location=871) ^ref-39312

---
Information hiding only makes sense when the information being hidden is not needed outside its module. If the information is needed outside the module, then you must not hide it. — location: [873](kindle://book?action=open&asin=B09B8LFKQL&location=873) ^ref-12347

---
if a module can automatically adjust its configuration, that is better than exposing configuration parameters. — location: [877](kindle://book?action=open&asin=B09B8LFKQL&location=877) ^ref-40910

---
When decomposing a system into modules, try not to be influenced by the order in which operations will occur at runtime; that will lead you down the path of temporal decomposition, — location: [883](kindle://book?action=open&asin=B09B8LFKQL&location=883) ^ref-2778

---
Instead, think about the different pieces of knowledge that are needed to carry out the tasks of your application, — location: [884](kindle://book?action=open&asin=B09B8LFKQL&location=884) ^ref-10290

---
I have found over and over that specialization leads to complexity; I now think that over-specialization may be the single greatest cause of complexity in software. — location: [893](kindle://book?action=open&asin=B09B8LFKQL&location=893) ^ref-32094

---
When designing modules such as classes or methods, one of the best ways to produce a deep API is to make it general-purpose — location: [895](kindle://book?action=open&asin=B09B8LFKQL&location=895) ^ref-19184

---
When writing detailed code, one of the most effective ways to simplify the code is by eliminating special cases, so that the common-case code handles the edge cases as well. — location: [896](kindle://book?action=open&asin=B09B8LFKQL&location=896) ^ref-47602

---
It turns out that even if you use a class in a special-purpose way, it’s less work to build it in a general-purpose way. — location: [914](kindle://book?action=open&asin=B09B8LFKQL&location=914) ^ref-52227

---
The phrase “somewhat general-purpose” means that the module’s functionality should reflect your current needs, but its interface should not. Instead, the interface should be general enough to support multiple uses. — location: [917](kindle://book?action=open&asin=B09B8LFKQL&location=917) ^ref-21935

---
don’t get carried away and build something so general-purpose that it is difficult to use for your current needs. — location: [920](kindle://book?action=open&asin=B09B8LFKQL&location=920) ^ref-50845

---
The text class ended up with a large number of shallow methods, each of which was only suitable for one user interface operation. — location: [940](kindle://book?action=open&asin=B09B8LFKQL&location=940) ^ref-27239

---
better approach is to make the text class more generic. Its API should be defined only in terms of basic text features, without reflecting the higher-level operations that will be implemented with it. — location: [949](kindle://book?action=open&asin=B09B8LFKQL&location=949) ^ref-19185

---
The first method inserts an arbitrary string at an arbitrary position within the text, and the second method deletes all of the characters at positions greater than or equal to start but less than end. — location: [953](kindle://book?action=open&asin=B09B8LFKQL&location=953) ^ref-31636

---
text.delete(cursor, text.changePosition(cursor, 1)); — location: [965](kindle://book?action=open&asin=B09B8LFKQL&location=965) ^ref-53801

---
Similarly, the backspace key can be implemented as follows: text.delete(text.changePosition(cursor, -1), cursor); — location: [966](kindle://book?action=open&asin=B09B8LFKQL&location=966) ^ref-8534

---
What is the simplest interface that will cover all my current needs? — location: [996](kindle://book?action=open&asin=B09B8LFKQL&location=996) ^ref-12644

---
If you reduce the number of methods in an API without reducing its overall capabilities, then you are probably creating more general-purpose methods. — location: [997](kindle://book?action=open&asin=B09B8LFKQL&location=997) ^ref-14760

---
Reducing the number of methods makes sense only as long as the API for each individual method stays simple; if you have to introduce lots of additional arguments in order to reduce the number of methods, then you may not really be simplifying things. — location: [1000](kindle://book?action=open&asin=B09B8LFKQL&location=1000) ^ref-25164

---
In how many situations will this method be used? — location: [1002](kindle://book?action=open&asin=B09B8LFKQL&location=1002) ^ref-40422

---
If a method is designed for one particular use, such as the backspace method, that is a red flag that it may be too special-purpose. See if you can replace several special-purpose methods with a single general-purpose method. — location: [1002](kindle://book?action=open&asin=B09B8LFKQL&location=1002) ^ref-13031

---
Is this API easy to use for my current needs? — location: [1004](kindle://book?action=open&asin=B09B8LFKQL&location=1004) ^ref-8286

---
If you have to write a lot of additional code to use a class for your current purpose, that’s a red flag that the interface doesn’t provide the right functionality. — location: [1006](kindle://book?action=open&asin=B09B8LFKQL&location=1006) ^ref-20607

---
specialized code should be cleanly separated from general-purpose code. — location: [1014](kindle://book?action=open&asin=B09B8LFKQL&location=1014) ^ref-37839

---
special cases should be eliminated wherever possible. — location: [1102](kindle://book?action=open&asin=B09B8LFKQL&location=1102) ^ref-5677

---
The best way to do this is by designing the normal case in a way that automatically handles the edge conditions without any extra code. — location: [1103](kindle://book?action=open&asin=B09B8LFKQL&location=1103) ^ref-60575

---
In a well-designed system, each layer provides a different abstraction from the layers above and below it; if you follow a single operation as it moves up and down through layers by invoking methods, the abstractions change with each method call. — location: [1123](kindle://book?action=open&asin=B09B8LFKQL&location=1123) ^ref-59812

---
If a system contains adjacent layers with similar abstractions, this is a red flag that suggests a problem with the class decomposition. — location: [1131](kindle://book?action=open&asin=B09B8LFKQL&location=1131) ^ref-30134

---
When adjacent layers have similar abstractions, the problem often manifests itself in the form of pass-through methods. — location: [1134](kindle://book?action=open&asin=B09B8LFKQL&location=1134) ^ref-46013

---
pass-through method is one that does nothing except pass its arguments to another method, usually with the same API as the pass-through method. This typically indicates that there is not a clean division of responsibility between the classes. — location: [1162](kindle://book?action=open&asin=B09B8LFKQL&location=1162) ^ref-58735

---
Pass-through methods make classes shallower: they increase the interface complexity of the class, which adds complexity, but they don’t increase the total functionality of the system. — location: [1165](kindle://book?action=open&asin=B09B8LFKQL&location=1165) ^ref-63601

---
Figure — location: [1177](kindle://book?action=open&asin=B09B8LFKQL&location=1177) ^ref-48516

---
One approach, shown in Figure 7.1(b), is to expose the lower level class directly to the callers of the higher level class, removing all responsibility for the feature from the higher level class. — location: [1177](kindle://book?action=open&asin=B09B8LFKQL&location=1177) ^ref-43800

---
Another approach is to redistribute the functionality between the classes, as in Figure 7.1(c). — location: [1179](kindle://book?action=open&asin=B09B8LFKQL&location=1179) ^ref-63370

---
Finally, if the classes can’t be disentangled, the best solution may be to merge them as in Figure 7.1(d). — location: [1179](kindle://book?action=open&asin=B09B8LFKQL&location=1179) ^ref-27078

---
The important thing is that each new method should contribute significant functionality. — location: [1185](kindle://book?action=open&asin=B09B8LFKQL&location=1185) ^ref-32439

---
The signature for the dispatcher is often the same as the signature for the methods that it calls. Even so, the dispatcher provides useful functionality: — location: [1188](kindle://book?action=open&asin=B09B8LFKQL&location=1188) ^ref-31726

---
For example, when a Web server receives an incoming HTTP request from a Web browser, it invokes a dispatcher that examines the URL in the incoming request and selects a specific method to handle the request. — location: [1194](kindle://book?action=open&asin=B09B8LFKQL&location=1194) ^ref-46661

---
It is fine for several methods to have the same signature as long as each of them provides useful and distinct functionality. — location: [1198](kindle://book?action=open&asin=B09B8LFKQL&location=1198) ^ref-5198

---
Another example is interfaces with multiple implementations, such as disk drivers in an operating system. Each driver provides support for a different kind of disk, but they all have the same interface. — location: [1199](kindle://book?action=open&asin=B09B8LFKQL&location=1199) ^ref-49447

---
A decorator object takes an existing object and extends its functionality; it provides an API similar or identical to the underlying object, and its methods invoke the methods of the underlying object. — location: [1205](kindle://book?action=open&asin=B09B8LFKQL&location=1205) ^ref-59869

---
The motivation for decorators is to separate special-purpose extensions of a class from a more generic core. However, decorator classes tend to be shallow: they introduce a large amount of boilerplate for a small amount of new functionality. — location: [1214](kindle://book?action=open&asin=B09B8LFKQL&location=1214) ^ref-17865

---
Decorator classes often contain many pass-through methods. It’s easy to overuse the decorator pattern, creating a new class for every small new feature. This results in an explosion of shallow classes, — location: [1216](kindle://book?action=open&asin=B09B8LFKQL&location=1216) ^ref-10191

---
Could you add the new functionality directly to the underlying class, — location: [1218](kindle://book?action=open&asin=B09B8LFKQL&location=1218) ^ref-19474

---
If the new functionality is specialized for a particular use case, would it make sense to merge it with the use case, rather than creating a separate class? — location: [1222](kindle://book?action=open&asin=B09B8LFKQL&location=1222) ^ref-22792

---
Could you merge the new functionality with an existing decorator, rather than creating a new decorator? — location: [1223](kindle://book?action=open&asin=B09B8LFKQL&location=1223) ^ref-42670

---
Finally, ask yourself whether the new functionality really needs to wrap the existing functionality: could you implement it as a stand-alone class that is independent of the base class? — location: [1225](kindle://book?action=open&asin=B09B8LFKQL&location=1225) ^ref-19493

---
rule is that the interface of a class should normally be different from its implementation: — location: [1232](kindle://book?action=open&asin=B09B8LFKQL&location=1232) ^ref-15364

---
Another form of API duplication across layers is a pass-through variable, which is a variable that is passed down through a long chain of methods. — location: [1247](kindle://book?action=open&asin=B09B8LFKQL&location=1247) ^ref-1435

---
Pass-through variables add complexity because they force all of the intermediate methods to be aware of their existence, even though the methods have no use for the variables. — location: [1253](kindle://book?action=open&asin=B09B8LFKQL&location=1253) ^ref-45538

---
challenging. One approach is to see if there is already an object shared between the topmost and bottommost methods. — location: [1256](kindle://book?action=open&asin=B09B8LFKQL&location=1256) ^ref-51184

---
However, if there is such an object, then it may itself be a pass-through variable (how else does m3 get access to it?). — location: [1262](kindle://book?action=open&asin=B09B8LFKQL&location=1262) ^ref-65053

---
Another approach is to store the information in a global variable, — location: [1263](kindle://book?action=open&asin=B09B8LFKQL&location=1263) ^ref-13445

---
but global variables almost always create other problems. — location: [1264](kindle://book?action=open&asin=B09B8LFKQL&location=1264) ^ref-35507

---
The solution I use most often is to introduce a context object as in Figure 7.2(d). A context stores all of the application’s global state (anything that would otherwise be a pass-through variable or global variable). Most applications have multiple variables in their global state, representing things such as configuration options, shared subsystems, and performance counters. There is one context object per instance of the system. The context allows multiple instances of the system to coexist in a single process, each with its own context. — location: [1267](kindle://book?action=open&asin=B09B8LFKQL&location=1267) ^ref-46731

---
Unfortunately, the context will probably be needed in many places, so it can potentially become a pass-through variable. — location: [1280](kindle://book?action=open&asin=B09B8LFKQL&location=1280) ^ref-52888

---
a reference to the context can be saved in most of the system’s major objects. — location: [1281](kindle://book?action=open&asin=B09B8LFKQL&location=1281) ^ref-55575

---
The context object unifies the handling of all system-global information and eliminates the need for pass-through variables. — location: [1285](kindle://book?action=open&asin=B09B8LFKQL&location=1285) ^ref-4265

---
Contexts are far from an ideal solution. The variables stored in a context have most of the disadvantages of global variables; for example, it may not be obvious why a particular variable is present, or where it is used. — location: [1290](kindle://book?action=open&asin=B09B8LFKQL&location=1290) ^ref-14200

---
the best way to avoid problems is for variables in a context to be immutable. — location: [1293](kindle://book?action=open&asin=B09B8LFKQL&location=1293) ^ref-13607

---
should you let users of the module deal with the complexity, or should you handle the complexity internally within the module? If the complexity is related to the functionality provided by the module, then the second answer is usually the right one. — location: [1305](kindle://book?action=open&asin=B09B8LFKQL&location=1305) ^ref-60628

---
is more important for a module to have a simple interface than a simple implementation. — location: [1309](kindle://book?action=open&asin=B09B8LFKQL&location=1309) ^ref-11592

---
Configuration parameters are an example of moving complexity upwards instead of down. — location: [1329](kindle://book?action=open&asin=B09B8LFKQL&location=1329) ^ref-53115

---
configuration parameters also provide an easy excuse to avoid dealing with important issues and pass them on to someone else. — location: [1337](kindle://book?action=open&asin=B09B8LFKQL&location=1337) ^ref-63510

---
transport protocol could compute a reasonable value on its own by measuring the response time for requests that succeed and then using a multiple of this for the retry interval. This approach pulls complexity downward and saves users from having to figure out the right retry interval. — location: [1341](kindle://book?action=open&asin=B09B8LFKQL&location=1341) ^ref-19528

---
you should avoid configuration parameters as much as possible. — location: [1345](kindle://book?action=open&asin=B09B8LFKQL&location=1345) ^ref-4774

---
When you do create configuration parameters, see if you can provide reasonable defaults, so users will only need to provide values under exceptional conditions. — location: [1346](kindle://book?action=open&asin=B09B8LFKQL&location=1346) ^ref-45878

---
Pulling complexity down makes the most sense if (a) the complexity being pulled down is closely related to the class’s existing functionality, (b) pulling the complexity down will result in simplifications elsewhere in the application, and (c) pulling the complexity down simplifies the class’s interface. — location: [1351](kindle://book?action=open&asin=B09B8LFKQL&location=1351) ^ref-45835

---
When deciding whether to combine or separate, the goal is to reduce the complexity of the system as a whole and improve its modularity. — location: [1367](kindle://book?action=open&asin=B09B8LFKQL&location=1367) ^ref-46537

---
Some complexity comes just from the number of components: the more components, the harder to keep track of them all and the harder to find a desired component within the large collection. — location: [1370](kindle://book?action=open&asin=B09B8LFKQL&location=1370) ^ref-48392

---
Subdivision can result in additional code to manage the components. — location: [1372](kindle://book?action=open&asin=B09B8LFKQL&location=1372) ^ref-57157

---
Subdivision creates separation: the subdivided components will be farther apart than they were before subdivision. — location: [1374](kindle://book?action=open&asin=B09B8LFKQL&location=1374) ^ref-3718

---
hand, if there are dependencies between the components, then separation is bad: developers will end up flipping back and forth between the components. — location: [1378](kindle://book?action=open&asin=B09B8LFKQL&location=1378) ^ref-44399

---
Subdivision can result in duplication: — location: [1379](kindle://book?action=open&asin=B09B8LFKQL&location=1379) ^ref-4027

---
Bringing pieces of code together is most beneficial if they are closely related. — location: [1381](kindle://book?action=open&asin=B09B8LFKQL&location=1381) ^ref-4516

---
Here are a few indications that two pieces of code are related: — location: [1382](kindle://book?action=open&asin=B09B8LFKQL&location=1382) ^ref-60113

---
They share information; — location: [1382](kindle://book?action=open&asin=B09B8LFKQL&location=1382) ^ref-27894

---
They are used together: anyone using one of the pieces of code is likely to use the other as well. — location: [1383](kindle://book?action=open&asin=B09B8LFKQL&location=1383) ^ref-33122

---
This form of relationship is only compelling if it is bidirectional. — location: [1384](kindle://book?action=open&asin=B09B8LFKQL&location=1384) ^ref-14467

---
They overlap conceptually, in that there is a simple higher-level category that includes both of the pieces of code. — location: [1385](kindle://book?action=open&asin=B09B8LFKQL&location=1385) ^ref-52927

---
It is hard to understand one of the pieces of code without looking at the other. — location: [1388](kindle://book?action=open&asin=B09B8LFKQL&location=1388) ^ref-52766

---
Bring together if information is shared — location: [1390](kindle://book?action=open&asin=B09B8LFKQL&location=1390) ^ref-12266

---
Because of this shared information, it is better to both read and parse the request in the same place; when the two classes were combined into one, the code got shorter and simpler. — location: [1396](kindle://book?action=open&asin=B09B8LFKQL&location=1396) ^ref-4817

---
Bring together if it will simplify the interface — location: [1398](kindle://book?action=open&asin=B09B8LFKQL&location=1398) ^ref-1065

---
This often happens when the original modules each implement part of the solution to a problem. — location: [1400](kindle://book?action=open&asin=B09B8LFKQL&location=1400) ^ref-23056

---
Bring together to eliminate duplication — location: [1409](kindle://book?action=open&asin=B09B8LFKQL&location=1409) ^ref-58682

---
If you find the same pattern of code repeated over and over, see if you can reorganize the code to eliminate the repetition. — location: [1409](kindle://book?action=open&asin=B09B8LFKQL&location=1409) ^ref-35626

---
This approach is most effective if the repeated code snippet is long and the replacement method has a simple signature. If the snippet is only one or two lines long, there may not be much benefit in replacing it with a method call. — location: [1411](kindle://book?action=open&asin=B09B8LFKQL&location=1411) ^ref-25361

---
If the snippet interacts in complex ways with its environment (such as by accessing numerous local variables), then the replacement method might require a complex signature (such as many pass-by-reference arguments), which would reduce its value. — location: [1412](kindle://book?action=open&asin=B09B8LFKQL&location=1412) ^ref-59773

---
Another way to eliminate duplication is to refactor the code so that the snippet in question only needs to be executed in one place. — location: [1414](kindle://book?action=open&asin=B09B8LFKQL&location=1414) ^ref-15806

---
Separate general-purpose and special-purpose code — location: [1422](kindle://book?action=open&asin=B09B8LFKQL&location=1422) ^ref-20202

---
If a module contains a mechanism that can be used for several different purposes, then it should provide just that one general-purpose mechanism. — location: [1422](kindle://book?action=open&asin=B09B8LFKQL&location=1422) ^ref-46049

---
It should not include code that specializes the mechanism for a particular use, nor should it contain other general-purpose mechanisms. — location: [1423](kindle://book?action=open&asin=B09B8LFKQL&location=1423) ^ref-59041

---
Special-purpose code associated with a general-purpose mechanism should normally go in a different module (typically — location: [1424](kindle://book?action=open&asin=B09B8LFKQL&location=1424) ^ref-4344

---
If the same piece of code (or code that is almost the same) appears over and over again, that’s a red flag that you haven’t found the right abstractions. — location: [1431](kindle://book?action=open&asin=B09B8LFKQL&location=1431) ^ref-59156

---
However, the combined object was awkward. It provided no benefit for higher-level code, since the higher-level code still needed to be aware of the selection and cursor as distinct entities, and it manipulated them separately — location: [1450](kindle://book?action=open&asin=B09B8LFKQL&location=1450) ^ref-976

---
new Position class was introduced to represent a location in the file (a line number and character within line). The selection was represented with two Positions and the cursor with one. Positions also found other uses in the project. — location: [1459](kindle://book?action=open&asin=B09B8LFKQL&location=1459) ^ref-49089

---
This red flag occurs when a general-purpose mechanism also contains code specialized for a particular use of that mechanism. This makes the mechanism more complicated and creates information leakage between the mechanism and the particular use case: future modifications to the use case are likely to require changes to the underlying mechanism as well. — location: [1465](kindle://book?action=open&asin=B09B8LFKQL&location=1465) ^ref-13942

---
This separation added complexity with no benefit. The logging methods were shallow: most consisted of a single line of code, but they required a considerable amount of documentation. Each method was only invoked in a single place. — location: [1499](kindle://book?action=open&asin=B09B8LFKQL&location=1499) ^ref-7923

---
it would be better to eliminate the logging methods and place the logging statements at the locations where the errors were detected. This would make the code easier to read and eliminate the interfaces required for the logging methods. — location: [1504](kindle://book?action=open&asin=B09B8LFKQL&location=1504) ^ref-63840

---
length by itself is rarely a good reason for splitting up a method. — location: [1510](kindle://book?action=open&asin=B09B8LFKQL&location=1510) ^ref-27027

---
Splitting up a method introduces additional interfaces, which add to complexity. — location: [1511](kindle://book?action=open&asin=B09B8LFKQL&location=1511) ^ref-10055

---
You shouldn’t break up a method unless it makes the overall system simpler; — location: [1512](kindle://book?action=open&asin=B09B8LFKQL&location=1512) ^ref-2764

---
Methods containing hundreds of lines of code are fine if they have a simple signature and are easy to read. These methods are deep (lots of functionality, simple interface), which is good. — location: [1518](kindle://book?action=open&asin=B09B8LFKQL&location=1518) ^ref-33338

---
When designing methods, the most important goal is to provide clean abstractions. Each method should do one thing and do it completely. — location: [1522](kindle://book?action=open&asin=B09B8LFKQL&location=1522) ^ref-44533

---
The method should have a simple interface, so that users don’t need to have much information in their heads in order to use it correctly. — location: [1523](kindle://book?action=open&asin=B09B8LFKQL&location=1523) ^ref-36568

---
The best way is by factoring out a subtask into a separate method, — location: [1527](kindle://book?action=open&asin=B09B8LFKQL&location=1527) ^ref-24607

---
The subdivision results in a child method containing the subtask and a parent method containing the remainder of the original method; the parent invokes the child. — location: [1527](kindle://book?action=open&asin=B09B8LFKQL&location=1527) ^ref-4264

---
The interface of the new parent method is the same as the original method. This form of subdivision makes sense if there is a subtask that is cleanly separable from the rest of the original method, which means (a) someone reading the child method doesn’t need to know anything about the parent method and (b) someone reading the parent method doesn’t need to understand the implementation of the child method. Typically this means that the child method is relatively general-purpose: it could conceivably be used by other methods besides the parent. — location: [1529](kindle://book?action=open&asin=B09B8LFKQL&location=1529) ^ref-41717

---
If you make a split of this form and then find yourself flipping back and forth between the parent and child to understand how they work together, that is a red flag (“Conjoined Methods”) indicating that the split was probably a bad idea. — location: [1532](kindle://book?action=open&asin=B09B8LFKQL&location=1532) ^ref-56498

---
The second way to break up a method is to split it into two separate methods, each visible to callers of the original method, as in Figure 9.3(c). This makes sense if the original method had an overly complex interface because it tried to do multiple things that were not closely related. — location: [1534](kindle://book?action=open&asin=B09B8LFKQL&location=1534) ^ref-43565

---
If you make a split like this, the interface for each of the resulting methods should be simpler than the interface of the original method. — location: [1538](kindle://book?action=open&asin=B09B8LFKQL&location=1538) ^ref-33996

---
Ideally, most callers should only need to invoke one of the two new methods; if callers must invoke both of the new methods, then that adds complexity, — location: [1539](kindle://book?action=open&asin=B09B8LFKQL&location=1539) ^ref-12132

---
If the caller has to invoke each of the separate methods, passing state back and forth between them, then splitting is not a good idea. — location: [1544](kindle://book?action=open&asin=B09B8LFKQL&location=1544) ^ref-16832

---
A more important issue is: does breaking up a function reduce the overall complexity of the system? In other words, is it easier to read several short functions and understand how they work together than it is to read one larger function? — location: [1564](kindle://book?action=open&asin=B09B8LFKQL&location=1564) ^ref-12312

---
The best way to eliminate exception handling complexity is to define your APIs so that there are no exceptions to handle: define errors out of existence. — location: [1669](kindle://book?action=open&asin=B09B8LFKQL&location=1669) ^ref-54001

---
The second technique for reducing the number of places where exceptions must be handled is exception masking. With this approach, an exceptional condition is detected and handled at a low level in the system, so that higher levels of software need not be aware of the condition. — location: [1718](kindle://book?action=open&asin=B09B8LFKQL&location=1718) ^ref-30278

---
The third technique for reducing complexity related to exceptions is exception aggregation. The idea behind exception aggregation is to handle many exceptions with a single piece of code; rather than writing distinct handlers for many individual exceptions, handle them all in one place with a single handler. — location: [1741](kindle://book?action=open&asin=B09B8LFKQL&location=1741) ^ref-32832

---
Try to pick approaches that are radically different from each other; — location: [1861](kindle://book?action=open&asin=B09B8LFKQL&location=1861) ^ref-10079

---
After you have roughed out the designs for the alternatives, make a list of the pros and cons of each one. — location: [1864](kindle://book?action=open&asin=B09B8LFKQL&location=1864) ^ref-2116

---
The most important consideration for an interface is ease of use for higher level software. — location: [1864](kindle://book?action=open&asin=B09B8LFKQL&location=1864) ^ref-9480

---
Does one alternative have a simpler interface than another? — location: [1868](kindle://book?action=open&asin=B09B8LFKQL&location=1868) ^ref-46639

---
Is one interface more general-purpose than another? — location: [1869](kindle://book?action=open&asin=B09B8LFKQL&location=1869) ^ref-5449

---
Does one interface enable a more efficient implementation than another? — location: [1870](kindle://book?action=open&asin=B09B8LFKQL&location=1870) ^ref-15041

---

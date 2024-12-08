Feathers, Michael C., Addison-Wesley, 2005

# Notes

## The source of code degradation

«Code can degrade in many ways, and many of them have nothing to do with whether the code came from another team.», pxvi

## Definition of Legacy Code

«To me, _legacy code_ is simply code without tests.», pxvi

## Tests as the gold standard of good code

«Code without tests is bad code. It doesn't matter how well written it is; it doesn't matter how pretty or object-oriented or well-encapsulated it is.», pxvi

## Tests as the teller of code improvement

«With tests, we can change the behavior of our code quickly and verifiable. Without them, we really don't know if our code is getting better or worse.», pxvi

## Tests are a safety net

«It is like doing aerial gymnastics without a net. It requires incredible skill and a clear understanding of what can happen at every step.», pxvi

## Code improvement doesn't happen over night

«it takes a long time for older code to get clearer.», pxvi

## The four reasons why software change

	1. Adding a feature
	2. Fixing a bug
	3. Improving the design
	4. Optimizing resource usage

page 3.

## The favorite excuse of developers

«"If they just stopped changing their minds, we'd be done by now"», p4

## Software is about behavior

«Behavior is the most important thing about software.», p4

## Adding code without changing behavior

«Adding a method doesn't change behavior unless the method is called somehow.», p5

## Dropping behavior introduces defects

«When we drop behavior in that process, we often call that a bug.», p5

## Why developers don't improve design

«One of the main reasons why many programmers don't attempt to improve design often is because it is relatively easy to loose behavior or create bad behavior in the process of doing it.», p5

## Refactoring

«The act of improving design without changing its behavior is called _refactoring_.», p5

## The idea behind refactoring

«The idea behind refactoring is that we can make software more maintainable without changing behavior.», p5

## How the refactoring process works

«we are making a series of small structural modifications, supported by tests to make the code easier to change.», p5

## Good vs Bad systems

«The difference between good systems and bad ones is that, in the good ones, you feel pretty calm after you've done that learning, and you are confident in the change you are about to make. In poorly structured code, the move from figuring things out to making changes feels like jumping off a cliff to avoid a tiger.», p8

## Change and fear

«The las consequence of avoiding change is fear.», p8

## Fear and avoidance

«We've talked about how avoiding change is a bad thing.», p8

## How Edit and Pray works

«When you use _Edit and Pray_, you carefully plan the changes you are going to make, you make sure that you understand the code you are going to modify, and then you start to make the changes. When you're done, you run the system to see if the change was enabled, and then you poke around further to make sure that you didn't break anything.», p9

## Working with care

«Superficially, _Edit and Pray_ seems like "working with care," a very professional thing to do. The "care" that you take is right there at the forefront, and you expend extra care when the changes are very invasive because much more can go wrong.», p9

## Working with care is useless

«Effective software change, like effective surgery, really involves deeper skills. Working with care doesn't do much for you if you don't use the right tools and techniques.», p9

## Cover and Modify

«_Cover and Modify_ is a different way of making changes. The idea behind it is that it is possible to work with a _safety net_ when we change software.», p9

## How Cover and Modify works

«Covering software means covering it with tests. When we have a good set of tests around a piece of code, we can make changes and find out very quickly whether the effects were good or bad.», p9

## Test to show correctness

«Testing done this way is really "testing to attempt to show correctness."», p10

## Regression testing

«In traditional terms, this is called regression testing. We periodically run tests that check for known good behavior to find out whether our software still works the way that it did in the past.», p10

## We lock behavior in place

«When we have tests that detect change, it is like having a vise around our code. The behavior of the code is fixed in place. When we make changes, we can know that we are changing only one piece of behavior at a time. In short, we're in control of our work.», p10

## Importance of unit tests

«Unit testing is one of the most important components in legacy code work.», p11

## What unit tests care about

«in unit testing, we are usually concerned with the most atomic behavioral units of a system.», p12

## Procedural systems and testing functions

«In procedural systems, it is often hard to test functions in isolation.», p12

## OO systems and testing

«In object-oriented systems, it is a little easier to test classes in isolation, but the fact is, classes don't generally live in isolation.», p12

## The importance of error localization

«As tests get further from what they test, it is harder to determine what a test failure means.», p12

## The importance of fast tests

«if our tests are large, execution time can be too long; our tendency will be to avoid running the tests often enough to really localize errors.», p13

## Qualities of good tests

	1. They run fast
	2. They help us localize problems

Page 13

## To cover or not to cover, that is the question

«The first thing to notice is that, given a choice, it is always safer to have tests around the changes that we make.», p14

## Legacy Code Dilemma

«When we change code, we should have tests in place. To put tests in place, we often have to change code.», p17

## Breaking dependencies safely

«When we break dependencies, we can often write tests that make more invasive changes safer. The trick is to do these initial refactorings very conservatively.», p17

## Being conservative while breaking dependencies

«Being conservative is the right thing to do when we can possibly introduce errors.», p17

## Ugly design as result of breaking dependencies

«When you break dependencies in legacy code, you often have to suspend your sense of aesthetics a bit. Some dependencies break cleanly; others end up looking less than ideal from a design point of view.», p18

## Legacy Code Change Algorithm

	1. Identify change points.
	2. Find test points.
	3. Break dependencies.
	4. Write tests.
	5. Make changes and refactor

Page 18

## Motivation behind the algorithm

«We wan to make functional changes that deliver value while bringing more of the system under test.», p18

## The end result of the algorithm

«At the end of each programming episode, we should be able to point not only to code that provides some new feature, but also its tests.», p18

## Why we need to break dependencies

«Dependencies are often the most obvious impediment to testing.», p19

## Another form of the legacy code paradox

«Often in legacy code, you have to break dependencies to get tests in place. Ideally, we should have tests that tell us wether the things we do to break dependencies cause problems, but often we don't.», p19

## Working on an ideal system

«Ideally, we wouldn't have to do anything special to a class to start working with it. In an ideal system, we'd be able to create objects of any class in a test harness and start working. We'd be able to create objects, write tests for them, and then move on to other things.», p21

## How we approach systems without tests

«In systems that weren't develop concurrently with unit tests, we often have to break dependencies to get classes into a test harness», p21

## Sensing and Separation

«Generally, when we want to get tests in place, there are two reasons to break dependencies: _sensing_ and _separation_.», p21

## Sensing

«We break dependencies to _sense_ when we can't access values our code computes.», p21

## Separation

«We break dependencies to _separate_ when we cant' even get a piece of code into a test harness to run.», p21

## When sensing is necessary

«We can't sense the effect of our class to methods on this class, and we can't run it separately from the rest of the application.», p22

## Fake objects and sensing

«there is one primary tool for sensing: fake collaborators.»

## Fake Objects

«A _fake object_ is an object that impersonates some collaborator of your class when it is being tested.», p23

## Mock Objects

«Mock objects are fakes that perform assertions internally.», p27

## Benefits of using mocks

«The nice thing about mocks is that we can tell them what calls to expect, and then we tell them to check anyd see if they received those calls.», p28

## Subtle dependencies

«Reuse is tough. Even when pieces of software look independent, they often depend upon each other in subtle ways.», p30

## Seam

«A seam is a place where you can alter behavior in your program without editing in that place.», p31

## Object Seam

«We were able to change the method that is called without changing the method that calls it.», p33

## Benefits of seams

«If we can replace behavior at seams, we can selectively exclude dependencies in our tests.», p33

## Seam implications

«When you have a seam, you have a place where behavior can change.», p36

## Enabling point

«Every seam has an enabling point, a place where you can make the decision to use one behavior or another.», p36

## Method call vs implementation

«The fundamental thing to recognize is that when we look at a call in an object-oriented program, it does not define which method will actually be executed.», p40

## Polymorphism

«Without knowing what object `cell` points to, we just don't know. It could be the `Recalculate` method of `ValueCell` or the `Recalculate` method of `FormulaCell`.», p41

## Not all methods are seams

«In object-oriented languages, not all method calls are seams.», p41

## Needed tools for working effectively with legacy code

«What tools do you need when you work with legacy code? You need an editor (or and IDE) and your build system, but you also need a testing framework.», p45

## Benefit of automatic refactoring tools

«Refactoring by hand is fine, but when you have a tool that does some refactoring for you, you have a real time saver.», p45

## When a change is a real refactor

«A change is a refactoring only if it doesn't change behavior. Refactoring tools should verify that a change does not change behavior, and many of them do.», p46

## Breaking dependencies and unit testing pays off

«the work that you do to break dependencies and write tests for your changes is going to take some time, but in most cases, you are going to end up saving time—and a lot of frustration.», p57

## Debugging is faster with tests

«With tests around the code, nailing down functional problems is often easier.», p57

## Changes cluster around

«Typically, changes cluster in systems. If you are changing it today, chances are, you'll have a change close by pretty soon.», p57

## The temptation of taking shortcuts

«When you don't really know how long it is going to take to add a feature and you suspect that it will be longer than the amount of time you have, it is tempting to just hack the feature in the quickest way that you can.», p59

## The "I'll add tests later" trap

«Then if you have enough time, you can go back and do some testing and refactoring. The hard part is actually going back and doing that testing and refactoring.», p59

## Sprout method

«When you need to add a feature to a system and it can be formulated completely as new code, write the code in a new method. Call it from the places where the new functionality needs to be.», p59

## Sprout method algorithm

	1. Identify where you need to make your code change.
	2. If the change can be formulated as a single sequence of statements in one place in a method, write down a call method that will do the work involved and then comment it out. (I like to do this before I even wreite the method so that I can get a sense of what the method call will look like in context.)
	3. Determine what local variables you need from the source method, and make them arguments to the call.
	4. Determine wether the sprouted method will need to return values to source method. If so, change the call so that its return value is assigned to a variable.
	5. Develop the sprout method using _test-driven development_.
	6. Remove the comment in the source method to enable the call.

Pages 61-62

## When to use the Sprout Method

«I recommend using _Sprout Method_ whenever you can see the code that you are adding as a distinct piece of work or you can't get tests around a method yet. It is far preferable to adding code inline.», p62

## Implication of using sprout method

«For one thing, when you use it, in effect you essentially are saying that you are giving up on the source method and its class for the moment.», p62

## Is about practical matters

«Giving up on a method or a class is the practical choice sometimes, but it still kind of sad.», p62

## Sprout method separates old from new method

«When you use _Sprout Method_, you are clearly separating new cod from old code.», p62-63

## Sprout Class

«Consider the case in which you have to make changes to a class, but there is just no way that you are going to be able to create objects of that class in a test harness in a reasonable amount of time, so there is no way to sprout a method and write tests for it on that class.», p63

## Sprout Classes and Class Genesis

«Some sprouted classes never fold back into the main concepts in the application. Instead, they become new ones.», p65

## First reason to use Sprout Class

«Essentially two cases lead us to _Sprout Class_. In one case, your changes lead you toward adding an entirely new responsibility to one of your classes.», p66

## Second reason to use Sprout Class

«The other case is the one we led off this chapter with. We have a small bit of functionality that we could place into an existing class, but we can't get the class into a test harness.», p66

## Advantage: Sprout Classes foment les invasive changes

«The key advantage of _Sprout Class_ is that it allows you to move forward with your work with more confidence than you could have if you were making invasive changes.», p67

## Disadvantage: more conceptual complexity

«The key disadvantage of _Sprout Class_ is conceptual complexity.», p67

## Why we are forced to use Sprout Class

«At other times, you move toward it only because your back is against the wall. Things that ideally would have stayed in that one class end up in sprouts just to make safe change possible.», p67

## Temporal coupling

«When you first create a method, it usually does just one thing for a client. Any additional code that you add later is sort of suspicious. Changes are, you're adding it just because it has to execute at the same time as the code you're adding it to. Back in the early days of programming, this was named _temporal coupling_, and it is a pretty nasty thing when you do it excessively.», p67

## Wrap Method

«When you need to add behavior, you can do it in a not-so-tangled way. One of the techniques that you can use is _Sprout Method_, but there is another that is very useful at times. I call it _Wrap Method_.», p67

## Why use wrap method

«_Wrap Method_ is a great way to introduce seams while adding new features.», p69

## Downside: introduce a new method name

«The second (and more real) downside is that you have to make up a new name for the old code that you had in the method.», p69

## Advantage of Wrap Method

«_Sprout Method_ and _Sprout Class_ add code to existing methods and make them longer by at least one line, but _Wrap Method_ does not increase the size of existing methods.», p70

## Another advantage

«Another advantage of _Wrap Method_ is that it explicitly makes the new functionality independent of existing functionality. When you wrap, you are not intertwining cod for one purpose with code for another.», p70

## Wrap Class

«_Wrap Class_ uses pretty much the same concept. If we need to add behavior in a system, we can add it to an existing method, but we can also add it to something else that uses that method. In _Wrap Class_, that something else is another class.», p71

## Wrap Class is a Decorator

«This technique is called the _decorator pattern_.», p72

## Benefits of Decorators

«Decorator allows you to build complex behaviors by composing objects at runtime.», p72

## Benefit of Wrap Class

«The key to _Wrap Class_ is that you are able to add new behavior into a system without adding it to an existing class.», p74

## Don't get discouraged

«If you spend most of your day wading through ugly code, it's very easy to believe that it will always be ugly and that any little thing that you do to make it better is simply not worth it.», p75

## Qualitative Change

«when you feel the difference between good code and bad code in your gut, you are a changed person. You might even find yourself wanting to refactor far in excess of what you need to get the job done, just to make your life easier.», p76

## Understanding and code size

«As the amount of code in a project grows, it gradually surpasses understanding.», p77

## Working in good vs bad systems

«In a well-maintained system, it might take a while to figure out how to make a change, but once you do, the change is usually easy and you feel much more comfortable with the system. In a legacy system, it can take a long time to figure out what to do, and the change is difficult also.», p77

## Manageable systems

«Systems that are broken up into small, well-named, understandable pieces enable faster work.», p78

## Lag Time

«La time is the amount of time that passes between a change that you make and the moment that you get real feedback about the change.», p78

## Independent modules

«You should be able to compile every class or module in your system separately from the others and in its own test harness.», p78

## Benefit of a small lag time

«We can use feedback to try out approaches quickly. Our work becomes more like driving than like waiting at a bus stop. Our concentration is more intense because we aren't constantly waiting for the next chance to do something.», p79

## Find the dependencies that get in the way

«In an object-oriented system, if you have a cluster of classes that you want to build more quickly, the first thing that you to figure out is which dependencies will get in the way.», p80

## Benefit of relying on interfaces

«When your code depends on an interface, that dependency is usually very minor and unobtrusive. Your code doesn't have to change unless the interface changes, and interfaces typically change far less often than the code behind them. When you have an interface, you can edit classes that implement that interface or add new classes that implement the interface, all without impacting code that uses the interface.», p84

## TDD is about doing one thing at a time

«One of the most valuable things about TDD is that it lets us concentrate one one thing at a time.», p94

## Programming by difference

«We can use inheritance to introduce features without modifying a class directly. After we've added the feature, we can figure out exactly how we really want the feature integrated.», p94

## Benefit of programming by difference

«_Programming by Difference_ lets us introduce variations quickly in systems.», p104

## Heuristic: just test it

«The best way to see if you will have trouble instantiating a class in a test harness is to just try to do it. Write a test case and attempt to create an object in it. The compiler will tell you what you need to make it really work.», p107

## Irritating Parameter

«The thing that is really getting in our way when we want to create the validator is the `RGHConnection`. It is an _irritating parameter_.», p108

## Extract Interface and Mock Objects

«In this case, the best way to make a fake object is to use `Extract Interace` (362) on the `RGHConnection` class.», p108

## Pass null

«If we don't need anything from them in the tests, we can `Pass Null`.», p131

## Test code vs Production code quality

«Test code doesn't have to live up to the same standards as production code.», p110

## Avoid passing Null

«The important thing to remember is this: Don't pass null in production code unless you have no other choice.», p111

## Breaking dependency technique: Extract Interface

«`Extract Interface` (362) is just one way of breaking a dependency on a parameter.», p135

## How to test a "hidden" method

«If we need to test a private method, we should make it public. If making it public bothers us, in most cases, it means that our class is doing too much and we ought to fix it.», p138

## Testeability as a property of good design

«Good design is testable, and design that isn't testable is bad.», p139

## Pain as friction for change

«the pain that we feel working in a legacy code base can be an incredible impetus to change.», p141

## Command/Query Seperation

«A method should be a command or a query, but not both.», p147

## What is a command

«A cmmand is a method that can modify the state of the object but that doesn't return a value.», p147

## What is a query

«A query is a method that returns a value but that does not modify the object.», p147

## Invisible bugs

«A change in one place can affect behavior someplace else; unless we have a test in place, we might never know about it.», p151

## Silent side-effects

«Effects can also propagate in silent, sneaky ways. If we have an object that accepts some object as a parameter, it can modify its state, and the change is reflected back into the rest of the application.», p164

## The case for encapsulation

«Encapsulation helps us reason about our code. In well-ensapsulated code, there are fewer paths to follow as you try to understand it.», p171

## Tests and understandability

«When we have test cases for a class, we can use them to reason about our code more directly.», p171

## Interception Points

«An _interception point_ is simply a point in your program where you can detect the effects of a particular change.», p174

## Verifying undesired changes in state

«Sometimes the only way you can be sure is by writing tests at the _interception point_ and then going back to the change point to alter the code a little bit and see if the tests fail.», p178

## Higher-Level Interception Points

«In most cases, the best _interception point_ we can have for a change is a public method on the class we're changing.», p178

## Pinch Point

«A _pinch point_ is a narrowing in an _effect sketch_, place where tests against a couple of methods can detect changes in many methods..», p181

## Pinch point as an encapsulation boundary

«A pinch point is a natural encapsulation boundary. When you find a _pinch point_, you've found a narrow funnel for all of the effects of a large piece of code.», p182

## When to use a pinch point

«Writing tests at _pinch points_ is an ideal way to start some invasive work in part of a program.», p183

## Analogy of Pinch points and owning a forest

«Test at a _pinch point_ are kind of like walking several steps int oa forest and drawing a line, saying "I own all this area." After you know that you own all of that area, you can develop it by refactoring and writing more tests. Over time, you can delete the tests at the _pinch point_ and let the tests for each class support your development work.», p184

## The point of regression testing

«automated tests should specify a goal that we'd like to fulfill or attempt to preserve behavior that is already there. In a natural flow of development, tests that _specify_ become tests that _preserver_.», p185

## Put the safety net in place first

«the best approach we can take when we need to make changes is to bolster the area we want to change with tests to provide some kind of safety net.», p185

## Bug finding tests vs characterization test

«If we write tests based on our assumption of what the system is supposed to do, we're back to bug finding again. Bug finding is important, but our goal right now is to get tests in place that help us make changes more deterministically.», p186

## Characterization tests

«A _characterization test_ is a test that characterizes the actual behavior of a piece of code.», p186

## Benefit of Characterization tests

«The tests document the actual current behavior of the system.», p186

## Characterization tests act as a Living documentation

«When we adopt this perspective, our view of our tests is different: They don't have any moral authority; they just sit there documenting what pieces of the system really does.», p188

## Unfamiliar code and fear

«Stepping into unfamiliar code, specially legacy code, can be scarey. Over time, some people become relatively immune to the fear. They develop confidence from confronting and slaying monsters in code over and over again, but it is tough not to be afraid. Everyone runs into demons that they can't slay from time to time.», p209

## Refactoring as a learning tool

«One of the best techniques for learning about code is refactoring. Just get in there and start moving things around and making the code clearer.», p212

## Scratch Refactoring

«Check out the code from your version-control system. Forget about writing tests. Extract methods, move variables, refactor it whatever way you want to get a better understanding of it—just don't check it in again. Throw that code away. This is called _Scratch refactoring_.», p212

## Benefits of Scratch Refactoring

«_Scratch refactoring_ is a great way of getting down the essentials and really learning how a piece of code works.», p212

## Systems decay over time

«Long-lived applications tend to sprawl. They might have started out with a well-thought-out architecture, but over the years, under schedule pressure, they can get to the point where nobody really understands their complete structure.», p215

## Oversimplified abstractions are not lies

«When you say that the simpler thing, it kind of feels like you are lying; you just aren't telling the whole story. But you are telling a simpler story that describes an easier-to-understand architecture.», p217

## The temptation of not creating new abstractions

«In legacy code, it's tempting to avoid creating abstractions. When I'm looking at four or five classes that have about a thousand lines of code apiece, I'm not thinking about adding new classes as much as I'm trying to figure out what has to change.», p224

## Code should reflect the conversations

«Software has to satisfy stronger constraints than just being easy to talk about, but if there isn't a strong overlap between conversation and code, it's important to ask why. The answer is usually a mixcture of two tings: The code hasn't been allowed to adapt to the team's understanding, or the team needs to understand it differently.», p224

## Procedural code and breaking dependencies

«Because breaking dependencies in procedural code is so hard, often the best strategy is to try to get a large chunk of the code under test before doing anything else and then use those tests to get some feedback while developing.», p231

## Strategy add new functions instead of extending existing ones

«In procedural legacy code, it pays to bias toward introducing new functions rather than adding code to old ones.», p236

## Benefit of encapsulation: code easier to reason about

«Clases that are too big often hide too much. Encapsulation is great when it helps us reason about code.», p246

## Over-encapsulation

«However, when we encapsulate too much, the stuff inside rots and festers.», p246

## How to deal with big classes

«The key remedy for big classes is refactoring. It helps us break down classes into sets of smaller classes.», p246

## Strategy: how to refactor big classes

«In real-world cases of big classes, the key is to identify the different responsibilities and then figure out a way to incrementally move toward more focused responsibilities», p249

## Technique: Method Grouping

«The key questions I asked were "Why is this method here?" and "What is it doing for the class?" Then I grouped them into lists, putting together methods that had a similar reason for being there.», p249

## Too many hidden methods hide new classes

«Pay attention to private and protected methods. If a class has many of them, it often indicates that there is another class in the class dying to get out.», p250

## When private methods should not be private

«if you have the urge to test a private method, the method shouldn't be private», p250

## Move methods into separate objects when they don't make sense as a public method

«if making the method publics bothers you, chances are, it is because it is part of a separate responsibility: it should be on another class.», p250

## Method names sometimes lie

«the names of methods don't tell the whole story. Often big classes house methods that do many things at many different levels of abstraction.», p251

## Class names should explain the responsibility of the class

«The _Single Responsibility Principle_ tells us that classes should have a single responsibility. If that's the case, it should have easy to write it down in a single sentence.», p260

## Interface Segregation Principle

«When a class is large, rarely do all of its client use all of its methods. Often we can see different groupings of methods that particular clients use. If we create an interface for each of these groupings and have the large class implement those interfaces, each client can see the bi class through that particular interface.», p263

## Benefits of Interface Segregation Principle

«This helps us hide information and also decreases dependency in the system.», p263

## Downside of Interface Segregation Principle

«Introducing SRP at the interface level requires more work. The clients of your class have to change, and you need tests for them.», p266

## Benefit of removing duplication: orthogonality

«When you remove duplication across classes, you end up with very small focused methods. Each of them does something that no other method does, and that gives us an incredible advantage: orthogonality.», p285

## Orthogonality

«Orthogonality is a fancy word for independence. If you want to change existing behavior in your code and there is exactly one place you have to go to make that change, you've got orthogonality.», p286

## Benefit of removing duplication: clear and flexible design

«Duplication removal is a powerful way of distilling a design. It not only makes a design more flexible, but it also makes changes faster and easier.», p287

## Monster Method

«Long methods are a pain, but monster methods are worse. A monster method is a method that is so long and so complex that you really don't feel comfortable touching it.», p289

## Technique: Out Method Object

«it epitomizes the idea of an invented abstraction. When you break out a method object, you create a class whose only responsibility is to do the work of your monster method.» p304

## Hyperaware Editing

«Hyperaware editing is a flow state, a state in which you can just shut out the world and work sensitively with the code.», p310

## Technique: Preserving Signatures

«One thing that I do is _Preserve Signatures_ whenever I can. When you cut/copy and paste entire method signatures from place to place you minimize any chance of errors.», p313

## Technique: Leaning on the compiler

«The key thing about this technique is that you are letting the compile guide you toward the changes you need to make. This doesn't mena that you stop thing about what you need to change; it just means that you can let the compiler do the legwork for you, in some cases.», p315

## How to thrive in legacy systems

«The key to thriving in legacy code is finding what motivates you.», p320

## Heuristic: solve the worst problem first to boost morale

«Pick the ugliest most obnoxious set of classes in the project, and get them under test. When you've tackled the worst problem as a team, you'll feel in control of your situation.», p321

## Breaking Dependencies Technique: Extract Interface

«_Extract Interface_ is often the best choice when it comes to breaking parameter dependencies.», p326

## Alternative: Adapt Parameter

«Use _Adapt Parameter_ when you can't use _Extract Interface_ on a parameter's class or when a parameter is difficult to fake.», p326

## Intention reviling interfaces

«Move toward interfaces that communicate responsibilities rather than implementation details. this makes code easier to read and easier to maintain.», p327

## The point of breaking dependencies

«remember that the goal is to break dependencies well enugh to get tests in place. Your bias should be toward making changes that you feel more confident in rather than changes that give you the best structure.», p328

## Safety (net) first

«Once you have tests in place, you can make invasive changes much more confidently.», p328

## Break Out Method Object

«In a nutshell, the idea behind this refactoring is to move a long method to a new class. Objects that you create using the new class are called method objects because they enbody the code of a single method.», p330

## Expose Static Method

«If you have a method that doesn't use instance data or methods, you can turn it into a static method. When it is static, you can get it under test without having to instantiate the class.», p345

## Lazy Getter

«A _lazy getter_ is a method that looks like a normal getter to all of tis callers. The key difference is that lazy getters create the object they are supposed to return the first time they are called.», p354

## Extract Interface is safe

«_Extract Interface_ is a one of the safest dependency-breaking techniques. If you get a step wrong, the compiler tells you immediately, so there is very little chance of introducing a bug.», p362

## Extract Interface explanation

«You create an interface for a class with declarations for all of the methods that you want to use in some context. When you've done that, you implement the interface to sense or separate, passing a fake object into the class you want to test.», p362

## Technique: Link Substitution

«Object orientation gives us wonderful opportunities to substitute one object for another. If two classes implement the same interface or have the same super-class, you can substitute one for another pretty easily.», p377

## Technique: Push Down Dependency

«When you use _Push Down Dependency_, you make your current class abstract. Then you create a subclass that will be your new production class, and push down all the problematic dependencies into that class.», p392

## Technique: Replace Global References with Getter

«One way to get past dependencies on globals in a class is to introduce getters for each of them in the class.», p399
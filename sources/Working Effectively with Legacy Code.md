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


# Bibliography
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

# Bibliography
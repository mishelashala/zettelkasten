Beck, Kent, Addison-Wesley, 2003

# Notes

## TDD is a style of development

«we drive development with automated tests, a style of development called Test-Driven Development», p ix

## Fear management

«Test-driven development is a way of managing fear during programming», p xi

## The feedback gap

«TDD is an awareness of the gap between decision and feedback during programming, and techniques to control that gap», p xii

## TDD is about confidence

«Test-driven development is a set of techniques that any software engineer can follow, which encourages simple designs and test suites that inspire confidence.», p xix

## A test is a concrete measure of failure

«Failure is progress. Now Now we have a concrete measure of failure», p5

## Dependencies and duplication

«If dependency is the problem, duplication is the symptom», p8

## Eliminating duplication

«eliminating duplication in programs eliminates dependency», p8

## TDD as an enabler of tiny steps

«TDD is not about taking teeny-tiny steps, it's about _being able_ to take teeny-tiny steps.», p9

## Value objects are immutable

«One implication of Value Objects is that all operations must return a new object», p15

## Tests as a precondition for refactoring

«Write the tests you wish you had. If you don't, you will eventually brea something while refactoring.», p29

## Just enough design

«Decide[d] not to introduce more design until we had a better motivation», p34

## Refactor technique: remove subclassing

«But because a constructor is not reason enough to have a subclass, we want to delete the subclasses», p51

## TDD doubles the amount of code

«You will likely end up with about the same number of lines of test code as model code when implementing TDD.», p78

## Frequently modified code should have solid tests

«If you have a big system, then the parts that you touch all the time should be absolutely rock solid, so you can make daily changes confidently.», p81

## Refactor technique: replace constants with variables

«take code that works in one instance and generalize it to work in many by replacing constants with variables.», p93

## Test coupling

«Test coupling has an obvious nasty effect, in that breaking one test causes the next ten to fial even though the code is correct.», p98

## Testing vs having tests

«Although you may test your changes, testing changes is not the same as _having_ tests.», p123

## Poor Management's Death Spiral

«The more stress you feel, the less testing you will do. The less testing you do, the more errors you will make. The more errors you make, the more stress you feel. Rinse and repeat.», p124

## Unit tests should be fast

«make the tests so fast to run that I can run them myself, and run them often.», p125

## Benefit of isolated tests

«One convenient implication of isolated tests is that tests are order independent. If I want to grab a subset of tests and run them, then I can do so without worrying that a test will break now because a prerequisite test is gone.», p125

## Benefits of testable code

«Isolating tests encourages you to compose solutions out of many highly cohesive, loosely coupled objects.», p125

## Evident Data

«How do you represent the intent of the data? Include expected and actual result in the test itself, and try to make their relationship apparent.», p130

## Shower Methodology

«If you know what to type, then type. If you don't know what to type, then take a shower, and stay in the shower until you know what to type.», p138

## Methodology for writing tests

«If you know what to type, type the Obvious Implementation. If you don't know what to type, then Fake It. If the right design still isn't clear, then Triangulate. If you _still_ don't know what to type, then you can take that shower.», p138

## Push thru it

«Sometimes when faced with a tough problem, what you need to do is press on, push through it.», p139

## You don't need DB for testing

«The solution is not to use a real database most of the time. Most tests are written in terms of and object that acts like a database, but is really just sitting in memory.», p144

## Rule of thumb: leave the last test broken

«How do you leave a programming session when you're programming alone? Leave the last test broken.», p148

## Tests reflect the stat of the program

«A broken test doesn't make the program any less finished, it just makes the status of the program manifest. The ability to pick up a thread of development quickly after weeks of hiatus is worth that little twinge of walking away from a red bar.», p149

## How to look at broken tests

«Once you have a broken test, you need to fix it. If you treat a red bar a s a condition to be fixed as quickly as possible, then you will discover that you can get to green quickly.», p151

## When to use Triangulation

«I only use Triangulation when I'm really, really unsure about the correct abstraction for the calculation. Otherwise I rely on either Obvious Implementation or Fake It.», p154

## How to use assertions

«How do you check that tests worked correctly? Write boolean expressions that automate your judgment about whether the code worked.», p157

## What boolean assertions represent

«The decisions have to be boolean—_True_ generally means everything is okay, and _false_ means something unexpected happened.», p157

## Fixtures

«How do you create common objects needed by several tests? Convert the local variables in the tests into instance variables. Override `setUp()` and initialize those variables.», p158

## Scaffolding

«Often you write more code setting objects up in an interesting state than you write manipulating them and checking results. The code for setting up the objects is the same for several tests (these objects are the tests's fixture, also known as scaffolding).», p159

## The goal while writing tests

«The goal of the game is to write the smallest test method that represents real progress toward your end goal.», p162

## Accidental Complexity

«One of the primary insights of patterns is that although it may seem as though we solve completely different problems all the time, most of the problems we solve are generated by the tools we use, not by the external problem at hand.», p165

## Command Object Pattern

«What do you do when you need the invocation of a computation to be more complicated than a simple method call? Make an object for the computation and invoke it.», p167

## Objects as organizers of logic

«Objects are a great way to organize logic for later understanding and growth.», p168

## Refactoring doesn't change semantics

«Usually, a refactoring cannot change the semantics of the program under any circumstances.», p181

## When to use Extract Method

«I use Extract Method to eliminate duplication when I see that two methods have some parts the same and some parts different.», p185

## Refactoring Technique: Extract Interface

«How do you introduce a second implementation of operations in Java? Create an interface containing the shared operations.», p187

## Testing Code Smell: Long Code Setup

«Long setup code—If you have to spend a hundred lines creating the objects for one simple assertion, then something is wrong. Your objects are too bing and need to be split.», p194

## Testing Code Smell: Setup Duplication

«Setup duplication—If you can't easily find a common place for common setup code, then there are too many objects too tightly intertwined.». p194

## TDD and Designing Ahead

«At the limit, where you introduce the variations very quickly, TDD is indistinguishable from designing ahead.», p196

## When not do delete a test

«Never delete a test if it reduces your confidence in the behavior of the system.», p198

## Repercussion of test last

«The biggest problem is that code that isn't written with tests in mind typically isn't very testable.», p200

## TDD increases confidence over time

«TDD enables you to gain confidence in the code over time. As tests accumulate (and your testing improves), you gain confidence in the behavior of the system.», p201

## TDD explains the impact of design 

«Another advantage of TDD that may explain its effect is the way it shortens the feedback loop on design decisions.», p203

# Bibliography

- Mandelbrot, Benoit, [[Fractals and Scaling in Finance]], New York, Springer Verlag, 1997
- McConnell, Steve, [[Code Complete]], Seattle, Washington, Microsoft Press, 1993
- Caine, S. H., and Gordon, E. K., [[PDL. A Tool for Software Design]], AFIPS, Proceedings of the 1975 National Computer Conference, 1975
- Alexander, Christopher, [[Notes on the Synthesis of Form]], Cambridge, Harvard University Press, 1970
- Gamma, Erich; Hel, Richard; Johnson, Ralph; Vlissides, John. [[Design Patterns. Elements of Reusable Object-Oriented Software]], Reading, Addison-Welsey, 1995
- Beck, K., [[The Smalltalk Best Practice Patterns]], Prentice-Hall, 1997
- Fowler, Martin, [[Refactoring. Improving the Design of Existing Code. 1st ed]], Reading, Addison-Wesley, 1999
- Weinberg, Gerald. [[Systems Thinking. Quality Software Management]], New York, 1992
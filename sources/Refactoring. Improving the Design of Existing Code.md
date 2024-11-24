## Notes

### Refactoring is not risk free

«Refactoring is risky. It requires changes to working code that can introduce subtle bugs.», pxi

### Refactoring is a serious endevour

«To avoid digging your own grave, refactoring must be done systematically.», pxi

### Definition of refactoring

«Refactoring is the process of changing a software system in a way that does not alter the external behavior of the code yet improves its internal structure.», xiv

### We can improve the situation

«With refactoring, we can take a bad, even chaotic, design and rework it into well-structured code.», pxiv

### Evolutionary Architectures

«I found that design, rather than occurring all up front, occurs continuously during development.», pxv

### Why poorly designed code is hard to change

«A poorly designed system is hard to change—because it is difficult to figure out what to change and how these changes will interact with the existing code to get the behavior I want.», p4

### Make the change easy, then make the easy change

«If the program lacks structure, it's usually easier for me to add structure to the program first, and then make the change I need.», p4

### When not to refactor

«If the code works and doesn't ever need to change, it's perfectly fine to leave it alone.», p5

### Tests are a precondition for refactoring

«Whenever I do refactoring, the first step is always the same. I need to ensure I have a solid set of tests for that section of code.», p5

### Tests as a bug catcher

«As I do the refactoring, I'll lean on the tests. I think of them as a bug detector to protect me against my own mistakes.», p5

### Tests as a double-check of correctness

«By writing what I want twice, in the code and in the test, I have to make the mistake consistently in both places to fool the detector. By double-checking my work, I reduce the chance of doing something wrong.», p5

### Always test after every refactor

«It's an important habit to test after every refactoring, however simple.», p8

### A lot of refactorings are the result of code not being clear enough

«As is often the case with refactoring, the early stages were mostly driven by trying to understand what was going.», p43

### Metric for good code

«I believe, however that we can go beyond taste and say that the true test of good code is how easy it is to change it.», p43

### Characteristics of a healthy code base

«A healthy code base maximizes our productivity, allowing us to build more features for our users both faster and more cheaply.», p43

### How to go faster with refactoring

«The key to effective refactoring is recognizing that you go faster when you take tiny steps, the code is never broken, and you can compose those small steps into substantial change.», p44

## Bibliography

- Scott W. Ambler and Pramod J. Sadalage. [[Refactoring Databases]], Addison-Wesley, 2006
- Jay Bazuzi, [[Safely Extract a Method in Any C++ Code]]
- Kent Beck, [[The Smalltalk Best Practice Patterns]], Addison-Wesley, 1997
- Michael Feathers, [[Working Effectively with Legacy Code]], Prentice Hall, 2004
- Kent Beck. [[Extreme Programming Explained]]. Addison-Wesley, 2005
- Jay Fields, Shane Harvie, and Martin Fowler. [[Refactoring Ruby Edition]]. Addison-Wesley, 2009
- Neal Ford, Rebecca Parsons, and Patrick Kua. [[Building Evolutionary Architectures]]. O'Reilly, 2017
- Nicole Forsgren, Jez Humble, and Gene Kim. [[Accelerate. The Science of Lean Software and DevOps. Building and Scaling High Performing Technology Organizations]]. IT Revolution Press, 2018
- Erich Gamma, Richard Helm, Ralph Johnson, and John Vlissides. [[Design Patterns. Elements of Reusable Object-Oriented Software]]. Addison-Wesley, 1994
- Elliotte Rusty Harold. [[Refactoring HTML]]. Addison-Wesley, 2008.
- Joshua Kerievsky. [[Refactoring to Patterns]], Addison-Wesley, 2004
- Gerard Meszaros. [[xUnit Test Patterns]]. Addison Wesley, 2007
- William F. Opdyke. [[Refactoring Object-Oriented Frameworks]]. Doctoral Dissertation. University of Illinois at Urbana-Champaign, 1992
- D. L. Parnas. “[[On the Criteria to Be Used in Decomposing Systems into Modules]]”. Communications of the ACM, Volume 15 Issue 12, pp. 1053-1058. Dec. 1972
- William C. Wake. [[Refactoring Workbook]]. Addison-Wesley, 2003.
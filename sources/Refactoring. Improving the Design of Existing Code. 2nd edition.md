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

«The key to effective refactoring is recognizing that you go faster when you take tiny steps, the code is never broken, and you can compose those small steps into substantial changes.», p44

### What refactoring is about

«Refactoring is all about applying small behavior preserving steps and making a big change by stringing together a sequence of these behavior-preserving steps.», p45

### Benefit: broken code for small periods of time

«As a result, when I'm refactoring my code doesn't spend much time in a broken state, allowing me to stop at any moment even if I haven't finished.», p46

### Refactoring is about observable behavior

«This is a deliberately loose term, indicating that the code should, overall, do just the same things it did before I started.», p46

### What refactoring is about

«Refactoring is always done to make the code "easier to understand and cheaper to modify".», p46

### Why to refactor

«Without refactoring, the internal design—the architecture—of software tends to decay.», p47

### Eliminating duplication and design

«an important aspect of improving design is to eliminate duplicated code.», p47

### Kent Beck about his skills and habits

«It reminds me of a statement Kent Beck often makes about himself: "I'm not a great programmer; I'm just a good programmer with great habits."», p48

### Design Stamina Hypothesis

«By putting our effort into a good internal design, we increase the stamina of the software effort, allowing us to go faster for longer.», p50

### Change and understanding

«Before I can change some code, I need to understand what it does.», p51

### Using tests to move understanding from the mind to the code

«As Ward Cunningham puts it, by refactoring I move the understanding from my head into the code itself. I then test that understanding by running the software to see if it still works.», p51

### Preserving knowledge in the code

«If I move my understanding into the code, it will be preserved longer and be visible to my colleges.», p51

### Refactoring as an understanding technique

«Then, as the code gets clearer, I find I can see things about the design that I could not see before.», p51

### Refactoring as a tool to reach higher levels of understanding

«When I'm studying code, refactoring leads me to higher levels of understanding that I would otherwise miss.», p51

### Software Paradigm: Accretion

«For a long time, people thought of writing software as a process of accretion:To add new features, we should be mostly adding new code.», p53

### Refactoring should not be dramatic

«Most refactoring effort should be the unremarkable, opportunistic kind.», p53

### Premise about code reviews

«Code reviews help spread knowledge through a development team.», p54

### Conclusion about code reviews

«The logical conclusion of this style is _pair programming_: continuous code review embedded within the process of programming.», p54

### Managers and refactoring

«To a manager who is genuinely savvy about technology and understands the design stamina hypothesis, refactoring isn't hard to justify. Such managers should be encouraging refactoring on a regular basis and be looking for signs that indicate a team isn't doing enough.», p55

### Too much vs too little refactoring

«While it does happen that teams do too much refactoring, it's much rarer than teams not doing enough.», p55

### When not to refactor

«If I run across code that is a mess, but I don't need to modify it, then I don't need to refactor it.», p55

### The purpose of refactoring

«The whole purpose of refactoring is to make use program faster, producing more value with less effort.», p56

### Refactoring is not driven by moral judgments

«I think the most dangerous way that people get trapped is when they try to justify refactoring in terms of "clean code," "good engineering practice," or similar moral reasons.», p56

### Refactoring is driven by economic incentives

«The point of refactoring isn't to show how sparkly a code base is—it is purely economic.», p56

### Refactoring is driven by speed

«We refactor because it makes us faster—faster to add features, faster to fix bugs.», p57

### Code ownership should be shared

«I recommend agains fine-grained strong code ownership. Some organizations like any piece of code to have a single programmer as an owner, and only allow that programmer to change it.», p57

### The rationale behind CI

«With CI, each team member integrates with mainline at least once per day. This prevents any branches diverting too far from each other and htus greatly reduces the complexity of merges.», p58

### Self-testing code is about catching bugs fast and early

«The key here is being able to catch an error quickly. To do this, realistically, I need to be able to run a comprehensive test suite on the code–and run it quickly, so that I'm not deterred from running it frequently. This means that in most cases, if I want to refactor, I need to have self-testing code.», p59

### Self-testing code enables bug catching and refactoring

«Self-testing code not only enables refactoring—it also makes it much safer to add new features, since I can quickly find and kill any bugs I introduce.», p59

### Refactoring little by little

«Even when I do have tests, I don't advocate trying to refactor a complicated legacy mess into beautiful code all at once. What I prefer to do is tackle it in relevant pieces. Each time I pass through a section of the code, I try to make it a little bit better—again.», p61

### How to refactor databases

«As with regular refactoring, the key here is that each individual change is small yet captures a complete change, so the system still runs after applying the migration.», p61

### Refactoring enables evolving architures

«The real impact of refactoring on architecture is in how it can be used to form a well-designed code base that can respond gracefully to changing needs.», p62

### Refactoring as a change-driving tool

«As my understanding of the user needs changes, I use refactoring to adapt the architecture to those new demands.», p62

### Always measure performance, don't speculate

«Even if you know exactly what is going on in your system, measure performance, don't speculate. You'll learn something, and nine times out of ten, it won't be that you were right!», p66

### The longer the function, the harder to understand

«Since the early days of programming, people have realized that the longer a function is, the more difficult it is to understand.», p73

### Heuristic: naming functions instead of explanations

«A heuristic we follow is that whenever we feel the need to comment something, we write a function instead. Such a function contains the code that we wanted to comment but is named after the _intention_ of he code rather than the way it works.», p73

### Rationale behind the heuristic

«A good technique is to look for comments. They often signal this kind of semantic distance. A block of code with a comment that tells you what it is doing can be replaced by a method whose name is based on the comment. Even a single line is worth extracting if it needs explanation.», p73

### Code Smell: Divergent Change

«Divergent change occurs when one module is often changed in different ways for different reasons.», p76

### Code Smell: Shotgun Surgery

«Shotgun surgery is similar to divergent change but is the opposite. You whiff this when, every time you make a change, you have to make a lot of little edits to a lot of different classes. When the changes are all over the place, they are hard to find, and it's easy to miss an important change.», p77

### Antidote to Divergent Changes

«The fundamental rule of thumb is to put things together that change together.», p77

### Code Smell: Primitive Obsession

«Strings are particularly common petri dishes for this kind of odor: A telephone number is more than just a collection of characters. If nothing else, a proper type can often include consistent display logic for when it needs to be displayed in a user interface. Representing such types as such a common stench that people call them "stringly typed" variables.», p78

### Polymorphism as an alternative to switch statements

«They'll argue that any switch statement you see is begging for _Replace Conditional with Polymorphism_.», p79

### Benefits of Immutable Data

«Immutable fields don't need to be encapsulated and information derived from immutable data can be represented as fields rather than getting methods.», 83

### Time division

«Some time is spent figuring out what ought to be going on, some time is spent designing, but most time is spent debugging.», p85

### Fixing vs finding a bug

«Fixing the bug is usually pretty quick, but finding it is a nightmare.», p85

### Test suits reduce debugging time

«A suite of tests is a powerful bug detector that decapitates the time it takes to find bugs.», p86

### Rule of thumb: run all tests at least once a day

«Run tests frequently. Run those exercising the code you're working on at least every few minutes; run all tests at least daily.», p92

### Testing is an iterative process

«Like most aspects of programming, testing is an iterative activity. Unless you are either very skilled or very lucky, you won't get your tests right the first time.», p93

### Heuristic: write test unit tests for bugs first

«When you get a bug report, start by writing a unit test that exposes the bug.», p99

### Code coverage does not guarantee quality

«test coverage analysis is only good for identifying untested areas of the code, not for assessing the quality of a test suite.», p99

### Over testing vs under testing

«Gut while over-testing does happen, it's vanishingly rare compared to under-testing.», p100

### Motivation behind the "extract to function" refactoring technique

«If you have to spend effort looking at a fragment of code and figuring out _what_ is doing, then you should extr act it into a function and name the function after the "what".», p107

### Side effect: plenty of small functions

«Once I accepted this principle, I developed a habit of writing very small functions—typically, only a few lines long.», p107

### Motivation behind "Extract Variable" refactoring method

«Expressions can become very complex and hard to read. In such situations, local variables my help break the expression down into something more manageable.», p119

### Motivation behind "Introduce Parameter Object" refactoring technique

«I often see groups of data items that regularly travel together, appearing in function after function. Such a group is a data clump, and I like to replace it with a single data structure.», p140

### Motivation behind "Combine Functions into Class" refactoring technique

«When I see a group of functions that operate closely together on a common body of data (usually passed as arguments to the function call), I see an opportunity to form a class.», p144

### Motivation behind "Split Phase" refactoring technique

«When I run into code that's dealing with two different things, I look for a way to split into a separate module.», p154

### Benefit of "Split Phase"

«Each step has a limited scope and I can think of one step without understanding the details of others.», p155

### Why decompose modules: to encapsulate

«Perhaps the most important criteria to be used in decomposing modules is to identify secrets that modules should hide from the rest of the system.», p161

### Motivation behind "Encapsulate Record" refactoring technique

«This is why I often favor objects over records for mutable data. With objects, I can hide what is stored and provide methods for all three values. The user of the object doesn't need to know or care which is stored and which is calculated.», p162

### Motivation behind "Encapsulate Collection" refactoring technique

«I like encapsulating any mutable data in my programs. This makes it easier to see when and how data structures are modified, which then makes it easier to change those data structures when I need to.», p170

### Motivation behind "Hide Delegate" refactoring technique

«Encapsulation means that modules need to know less about other parts of the system. Then, when things change, fewer modules need to be told about the change which makes the change easier to make.», p189

### Motivation behind "Move Function" refactoring technique

«The heart of a good software design is its modularity—which is my ability to make most modifications to a program wile only having to understand a small part of it.», p198

### How to achieve modularity

«To get this modularity, I need to ensure that related software elements are grouped together and the links between them are easy to find and understand.», p198

### Motivation behind "Move Statements into Function" refactoring technique

«If I see the same code executed every time I call a particular function, I look to combine that repeating code into the function itself.», p213

### Motivation behind "Replace Inline Code with Function Call" refactoring technique

«Functions allow me to package up bits of behavior. This is useful for understanding—a named function can explain the purpose of the code rather than its mechanic.», p222

### Motivation behind "Side Statements" refactoring technique

«Code is easier to understand when things that are related to each other appear together. If several lines of code access the same data structure, it's best for them to be together rather than intermingled with code accessing other data structures.», p223

### Motivation behind "Split Loop" refactoring techniques

«if you're doing two different things in the same loop, then whenever you need to modify the loop you have to understand both things.», p228

### Motivation behind "Remove Dead Code" refactoring technique

«unused code is still a significant burden when trying to understand how the software works.», p237

### Motivation behind "Replace Derived Variable with Query" refactoring technique

«Data changes can often couple together parts of code in awkward ways, with changes in one part leading to knock-on effects that are hard to spot. In many situations, it's not realistic to entirely remove mutable data—but I do advocate minimizing the scope of mutable data at much as possible.», p248

### Why value objects are easier to reason about

«Value objects are generally easier to reason about, particularly because they are immutable. In general, immutable data structures are easier to deal with.», p252

### Conditional logic: a common source of complexity

«One of the most common sources of complexity in a program is complex conditional logic.», p260

### How conditionals make code harder to understand

«The problem usually lies in the fact that the code, both in the condition checks and problem usually lies in the fact that the code, both in the condition checks and in the actions, tells me what happens but can easily obscure _why_ it happens.», p260

### Motivation behind "Consolidate Conditional Expression" refactoring technique

«Sometimes, I run into a series of conditional checks where each check is different yet the resulting action is the same. When I see this, I use _and_ and _or_ operators to consolidate them into a single conditional check with a single result.», p263

### What is an assertion

«An assertion is a conditional statement that is assumed to be always true.», p302

### What assertions indicated

«Failure of an assertion indicates a programmer error. Assertion failures should never be checked by other parts of the system. Assertions should be written so that the program functions equally correctly if they are all removed; indeed, some languages provide assertions that can be disabled by a compile-time switch.», p302

### Element of a good API

«A good API clearly separates any functions that update data from those that only read data.», p305

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
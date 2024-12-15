## Notes

### What the term "Refactoring to Patterns" imply

«_Refactoring to Patterns_ suggests that using patterns to improve an existing design is better than using patterns early in a new design.», pxix

### How over-engineered code affects productivity

«Over-engineered code affects productivity because when programmers inherit and over-engineered design, they must sped time learning the nuances of that design before they can comfortably extend or maintain it.», p2

### One reason behind over-engineered code

«Perhaps the main reason programmers over-engineer is that they don't want to get stuck with a bad design.», p2

### Principles vs Patterns

«Experiences like this made me aware that I needed to top thinking so much about patterns and refocus on writing small, simple, understandable code.», p3

### Under-engineering vs Over-engineering

«Under-engineering is far more common than over-engineering.», p3

### When we under-engineer

«We under-engineer when we produce poorly designed software.», p3

### Refactoring and Patterns

«There is a natural relation between patterns and refactorings. Patterns are where you want to be; refactorings are ways to get there from somewhere else.»

> Note: the author is quoting Refactoring from Martin Fowler

### Understand the why, not the how

«I know that understanding good reasons to refactor to or towards a pattern are more valuable than understanding the end result of a pattern or the nuances of implementing that ned result.», p8

### How to keep a code base clean

«To keep code clean, we must continuously remove duplication and simplify and clarify code. We must not tolerate messes in code, and we must not backslide into bad habits.», p14

### The golden cycle of clean code

«Clean code leds to better design, which leads to faster development, which leads to happy customers and programmers. Keep your code clean.», p14

### Passing tests as a north start

«the green bar has become a gyroscope, a device that helps me stay on course. If the bar stays red for too long—more than a few minutes—I know that I'm not taking a small enough steps.», p15

### How design debt occurs

	Design debt occurs when you don't consistenly do three things:
	1. Remove duplication.
	2. Simplify your code.
	3. Clarify your code's intent

p16

### Composite refactorings

«**Composite refactorings** are high-level refactorings compose of low-level refactorings. Much of the work performed by low-level refactorings involves moving code around.», p17

### Patterns Happy

«The overuse of patterns tends to result from being patterns happy.», p24

### When we are patterns happy

«We are **patterns happy** when we become enamored of patterns that we simply must use them in our code. A patterns-happy programmer may work hard to use patterns on a system just to get the experience of implementing them or maybe to gain a reputation for writing really good, complex code.», p24

### Solution Sprawl Code Smell

«A class that is a Factory is one that implements one or more Creation Methods. If data and/or code used in object creation become sprawled across numerous classes, you'll likely find yourself frequently updating code in numerous places, a sure sign of the smell _Solution Sprawl_.», p55

### Creation Method

«A Creation Method can help make these problems go away. A Creation Method is simply a static or nonstatic method on a class that instantiates new instances of the class.», p58

### Creation Method vs Factory Method

«I'm using the term Creation Method to refer to a static or nonstatic method that creates instances of a class. This means that every Factory Method is a Creation Method but not necessarily the reverse.», p59

### When creation sprawl occurs

«When the knowledge for creating an object is spread out across numerous classes, you have **creation sprawl**», p69

### Motivation behind "Move Creation Knowledge to Factory" refactoring technique

«the placement of creational responsibilities in classes that ought not to be playing any role in an object's creation.», p69

### Why Factory Methods are common in OO programs

«Factory Methods are most common in object-oriented programs because they provide a way to make object creation polymorphic.», p89

### Benefit of using State Objects

«A context delegates state-dependent behavior to a state object. State objects make state transitions at runtime by making the context point to a different state object.», p167

### Definition of Generalization

«Generalization is the transformation of specific code into general-purpose code.», p203

### Generalization is often the product of refactoring

«The production of generalized code frequently occurs as a result of refactoring.», p203

### Motivations behind generalization

«The most common motivation for applying them is to remove duplicated code. A secondary motivation is to simplify or clarify code.», p203

### Motivation behind "Extract Composite" refactoring technique

«if you have two or more classes with similar features, it makes sense to move the common features to a super class.», p215

### Benefit of "Extract Composite"

«It lets clients process one or many objects with a single method.», p226

### Other benefit of "Extract Composite"

«In short, replacing a one/many distinct with a Composite is a way to remove duplication, make client class uniform, and support the processing of trees of objects.», p226

### Alternative Class with Different Interfaces code smell

«The smell _Alternative Class with Different Interfaces_ identifies when code could be communicating with alternative classes via a common interface but for some reason does not.», p248

### Motivation behind "Extract Adapter" refactoring technique

«I routinely encounter code that attempts to handled multiple versions of something by overloading classes with version-specific state variables, constructors, and methods.», p259

### How "Extract Adapter" works

«for each version of something you need to support, create a separate class.», p259

### Definition of Adapter Class

«Such classes are called Adapters. Adapters implement a common interface and are responsible for functioning correctly with one (and usually only one) version of some code.», p259

### Adapters vs Facades

«Adapters adapt objects, while Facades adapt entire subsystems.», p259

### Motivation behind Facades

«Facades are often used to communicate with legacy systems.», p260

### Where Facades shine 

«They provide new systems with simpler views of poorly designed or highly complex legacy code.», p260

### Facades and refactoring legacy systems

«Over time, teams can rewrite entire legacy subsystems by simply writing new implementations for each Facade.», p260

### Protection and refactoring

«A refactoring that improves the protection of existing code must do so in a way that doesn't alter the behavior of the existing code.», p285

### Refactorization and Premature Optimization

«Prematurely optimized code is harder to refactor than code that hasn't been optimized.», p296

### Singleton and Premature Optimization

«If you use the Singleton Pattern out of habit, because it "makes your code more efficient," you're prematurely optimizing.», p296

### Motivation behind "Introduce Null Object" refactoring technique

«Null logic also fails to provide null protections for new code. So if new code is written and programmers forget to include null logic for it, null errors can begin to occur.», p302

### Null Object solves the problem null pointer exceptions

«The _Null Object_ pattern provides a solution to such problems. It removes the need to check wether a field or variable is null by making it possible to _always_ call the field or variable safely.», p302

### Design Patterns and Refactoring

«Design patterns are the word problems of the programming world; refactoring is its algebra.», p349

## Bibliography

- Alexander Christopher, [[A Pattern Language]], New York, Oxford University Press, 1977
- Alexander, Christopher, [[A Timeless Way of Building]], New York, Oxford University Press, 1979
- Anderson, Bruce. "Null Object", UIUC Patterns Discussion Mailing List, January 1995
- Astels, David, [[Test-Driven Development, a Practical Guider]], Upper Saddle River, Prentice Hall, 2003
- Barzun, Jacques, [[Simple and Direct]], 4th ed., New York, HarperCollins, 2001
- Beck, Kent, [[The Smalltalk Best Practice Patterns]], Upper Saddle River, Prentice Hall, 1997
- Beck, Kent, [[Test-Driven-Development by Example]], Addison-Wesley, 2002
- Beck, Kent. [[Extreme Programming Explained]], Reading, Addison-Wesley, 1999
- Bloch, Joshua. [[Effective Java]], Boston, Addison-Wesley, 2001
- Cunningham, Ward, "Checks: A Pattern Language of Information Integrity". In [[Pattern Languages of Program Design]], eds. James O. Coplien and Douglas C. Schmidt. Reading, Addison-Wesley, 1995
- Gamma, Erich, Ricahrd Helm, Ralph Johnson, and John Vlissides. [[Design Patterns. Elements of Reusable Object-Oriented Software]], Reading, Addison-Wesley, 1995
- Evans, Eric. [[Domain-Driven Design. Tackling Complexity in the Heart of Software]], Addison-Wesley, 2003
- Foote, Brian, and oseph Yoder. "Big Ball of Mud.", In [[Pattern Languages of Program Design]], eds Neil Harrison, Brian Foote, and Hans Rohnert. Boston, Addison-Wesley, 2000
- Fowler, Martin. [[Refactoring. Improving the Design of Existing Code. 1st ed]], Boston, Addison-Wesley, 2000
- Fowler, Martin. [[Patterns of Enterprise Application Architecture]], Boston, Addison-Wesley, 2003
- Fowler, Martin. [[UML Distilled]], 3rd ed. Boston, Addison-Wesley, 2003
- Gamma, Erich, and Kent Beck. [[Contributing to Eclipse]], Boston, Addison-Wesley, 2003
- Kerievsky, Joshua. [[Pools of Insight. A Pattern Language for Study Groups]]
- Kerievsky, Joshua, "Patterns & XP", in [[Extreme Programming Explained]], eds., Giancarlo Succi and Michele Marchesi, Boston, Addison-Wesley, 2001
- Parnas, David. [[On the Criteria to Be Used in Decomposing Systems into Modules]], Communications of the ACM, 15(2), 1972
- Roberts, Don, John Brand, and Ralph Johnson. [[A Refactoring Tool for Smalltalk]]
- Solomon, Maynard. [[Mozart]], New York, HarperCollings, 1995
- Vlissides, John, [[C++ Report]], April 1998
- Woolf, Bobby. "The Null Object Pattern", In [[Pattern Languages of Program Design]], eds. Robert C. Martin, Dirk Riehle, and Frank Buschmann, Reading, Addison-Wesley, 1997
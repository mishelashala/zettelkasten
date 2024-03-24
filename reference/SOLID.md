## Benefits

### Slices allow parallel work

"Another benefit of this slicing style is that it makes parallel work on different operations a breeze. We won't have merge conflicts if two developers work on different operations."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p53

## Single responsibility principle

"A component should do only one thing and do it right."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p17

### Alternative definition

"A component should have only one reason to change."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p17

### Violating the SRP leads to code duplication

"If the responsibilities are so coupled that you cannot use just the behavior you need, you could duplicate the code of interest."

Sandi Metz, Practical Object-Oriented Design, p21

### How to know how many responsibilities a class has

"If the simplest description you can devise uses the word "and," the class likely has more than one responsibility."

Sandi Metz, Practical Object-Oriented Design, p22

## Open-Closed principle

## Liskov Substitution Principle

## Interface Segregation Principle

"[...] states that broad interfaces should be split into specific ones so that clients only know the methods they need."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p58

## Dependency Inversion Principle

"states that high-level components should not depend on low-level components. Instead, both of them should depend on abstractions."

Davi Vieira, Designin Hexagonal Architectures, p252

### DI Principle decouple classes

"Moving the creation of the new `Wheel` instance outside of `Gear` decouples the two classes. Gear can now collaborate with any object that implements `diameter`."

Sandi Metz, Practical Object-Oriented Design, p43

### High vs Low level

"The high-level component can be either a concrete or abstract element, while the low-level component should be concrete because it always provides implementation details."

Davi Vieira, Designin Hexagonal Architectures, p252

### High Level Component

"A high level component has a set of operations orchestrated to enable a major system behavior. A high-level component may rely on low-level components to provide a major system behavior."

Davi Vieira, Designin Hexagonal Architectures, p252

### Low Level Component

"A low-level component, in turn, utilizes a specialized behavior that supports the goal of a high-level component."

Davi Vieira, Designin Hexagonal Architectures, p252

### How to invert a dependency

"To invert the dependency, we need to make the high-level component depend on the same abstraction that the low-level component is derived from. In object-oriented designs, we can achieve this feat by using abstract classes or interfaces."

Davi Vieira, Designin Hexagonal Architectures, p253

### The problem with concrete classes

"When Gear hard-codes a reference to Wheel deep inside its gear_inches method, it is explicitly declaring that it is only willing to calculate gear inches for instances of Wheel. Gear refuses to collaborate with any other kind of object, even if that object has a diameter and uses gears."

Sandi Metz, Practical Object-Oriented Design, p42

### Object Message vs Class Names

"Using dependency injection to shape code relies on your ability to recognize that the responsibility for knowing the name of a class and the responsibility for knowing the name of a message to send to that class may belong in different objects."

Sandi Metz, Practical Object-Oriented Design, p43
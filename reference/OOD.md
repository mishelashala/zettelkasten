## What OOD is about

"Object-Oriented design is about managing dependencies. It is a set of coding techniques that arrange dependencies such that objects can tolerate change."

Sandi Metz, Practical Object-Oriented Design, p3

## Principle behind OOD

"One of the important principles of object-oriented design is that every computation must be represented as an application of a method on a given object, which is the treated as the current object for the computation."

Object-oriented Analysis, Design and Implementation, p162

## ODD is about blind trust

"This blind trust is a keystone of object-oriented design. It allows objects to collaborate without binding themselves to context and is necessary in any application that expects to grow and change."

Sandi Metz, Practical Object-Oriented Design, p75

## When objects know too much

"When objects know too much, they have many expectations about the world in which they reside. They're picky, they need things to be 'just so.' These expectations constrain them. The objects resist being reused in different contexts; they are painful to test and susceptible to being duplicated."

Sandi Metz, Practical Object-Oriented Design, p3

## Dependency Direction

### Why to invert the dependency direction

- Some classes are more likely than others to have changes in requirements.
- Concrete classes are ore likely to change than abstract classes.
- Changing a class that has many dependents will result in widespread consequences.

Sandi Metz, Practical Object Oriented Design, p55

## Abstractions

### Why to rely on abstractions

"The wonderful thing about abstractions is that they represent common, stable qualities. They are less likely to change than are the concrete classes from which they are extracted. Depending on an abstraction is always safer than depending on a concretion because by its very nature, the abstraction is more stable."

Sandi Metz, Practical Object Oriented Design, p57


# What OOD is about

"Object-Oriented design is about managing dependencies. It is a set of coding techniques that arrange dependencies such that objects can tolerate change."

Sandi Metz, Practical Object-Oriented Design, p3

# Principle behind OOD

"One of the important principles of object-oriented design is that every computation must be represented as an application of a method on a given object, which is the treated as the current object for the computation."

Object-oriented Analysis, Design and Implementation, p162

# ODD is about blind trust

"This blind trust is a keystone of object-oriented design. It allows objects to collaborate without binding themselves to context and is necessary in any application that expects to grow and change."

Sandi Metz, Practical Object-Oriented Design, p75

# The goal of OOD

"Your goal is to model your application, using classes, such that it does what it is supposed to do _right now_ and is also easy to change _later_."

Sandi Metz, Practical Object-Oriented Design, p15

# When objects know too much

"When objects know too much, they have many expectations about the world in which they reside. They're picky, they need things to be 'just so.' These expectations constrain them. The objects resist being reused in different contexts; they are painful to test and susceptible to being duplicated."

Sandi Metz, Practical Object-Oriented Design, p3

# How to recognize a dependency

"An object has a dependency when it knows:
- The name of another class. [...]
- The name of a message that it intends to send to someone other than self. [...]
- The arguments that message requires. [...]
- The order of those arguments [...]"

Sandi Metz, Practical Object-Oriented Design, p39

# Dependency Direction

## Why to invert the dependency direction

- Some classes are more likely than others to have changes in requirements.
- Concrete classes are ore likely to change than abstract classes.
- Changing a class that has many dependents will result in widespread consequences.

Sandi Metz, Practical Object Oriented Design, p55

# Abstractions

## Why to rely on abstractions

"The wonderful thing about abstractions is that they represent common, stable qualities. They are less likely to change than are the concrete classes from which they are extracted. Depending on an abstraction is always safer than depending on a concretion because by its very nature, the abstraction is more stable."

Sandi Metz, Practical Object Oriented Design, p57

# Data Types are Expectations

"In a procedural language, variables have a single data type; knowledge of this data type lets you have expectations about which operations are valid."

Sandi Metz, Practical Object-Oriented Design, p12

# Object Types Are Expectations

"Knowing an object's type lets you have expectations about how it will behave."

Sandi Metz, Practical Object-Oriented Design, p12

# The API is a contract

"The public interface is a contract the articulates the responsibilities of your class."

Sandi Metz, Practical Object-Oriented Design, p64

# Public Interface's Laws

- Reveal its primary responsibility.
- Are expected to be invoked by others.
- Will not change on a whim.
- Are safe for others to depend on.
- Are thoroughly documented in the tests.

Sandi Metz, Practical Object-Oriented Design, p64

# Private Interface's Laws

- Handle implementation details.
- Are not expected to be sent by other objects.
- Can change for any reason whatsoever.
- Are unsafe for others to depend on.
- May not even be referenced in the tests.

Sandi Metz, Practical Object-Oriented Design, p64

# Incoming vs outgoing messages

"The incoming messages make up the public interface of the receiving object. The outgoing messages, by definition, are incoming into other objects and so are part of some other object's interface."

Sandi Metz, Practical Object-Oriented Design, p197

# Small Methods

## Benefits

- Expose previously hidden qualities
- Avoid the need for comments
- Encourage reuse
- Are easy to move to another class

Sandi Metz, Practical Object-Oriented Design, p31-32

# Favor objects with simpler contexts

"The context that an object expects has a direct effect on how difficult it is to reuse. Objects that have a simple context are easy to use and easy to test; they expect few things from their surroundings."

Sandi Metz, Practical Object-Oriented Design, p73

# Small Objects are transparent

"[...] small objects have a single responsibility and specify their own behavior.
They are _transparent_; it's easy to understand the code and it's clear what will happen if it changes."

Sandi Metz, Practical Object-Oriented Design, p188
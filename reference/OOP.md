## What is an object

"Each component *(object)* represents a data abstraction and is designed to store information along with procedures to manipulate the same"

Object-Oriented Analysis, Design and Implementation, p5.

## What is a software system

"The overall philosophy here is to define a software system as a collection of objects of various types that interact with each other through well-defined interfaces."

Object-Oriented Analysis, Design and Implementation, p5.

## Software Adaptability

"The ability to change the functionality of a component allows for systems to be more adaptable"

Object-Oriented Analysis, Design and Implementation, p8

## Foundations of an OO system

"The foundation of an object-oriented system is the _message_, but the most visible organizational structure is the _class_."

Sandi Metz, Practical Object-Oriented Design, p15

## Distinctive characteristic of OOP

"What characterizes an object-oriented system is its ability to treat data and behavior as closely related."

Davi Vieira, Designing Hexagonal Architecture, p90

## OOP is about messages

"More than classes, inheritance, or encapsulation, the fundamental feature of an object oriented program is the sending of messages. Every action the program performs boils down to a series of messages sent to objects."

Avdi Grimm, Confident Ruby, p26

## OOP systems are defined by their messages

"[...] an object oriented application is more than just classes. It is made up of classes but _defined_ by messages."

Sandi Metz, Practical Object Oriented Design, p61

## Reusability

### Reusable Classes

"Reusable classes are pluggable units of well-defined behavior that have few entanglements. An application that is easy to change is like a box of building blocks; you can select just the pieces you need and assemble them in unanticipated ways."

Sandi Metz, Practical Object-Oriented Design, p21

### Reusable Objects

#### Reusable Objects are independent of context

"The best possible situation is for an object to be completely independent of its context. An object that could collaborate with others without knowing who they are or what they do could be reused in novel and unanticipated ways."

Sandi Metz, Practical Object-Oriented Design, p73

#### Removing vs Isolating dependencies

"[...] if you cannot remove unnecessary dependencies, you should isolate them within your class."

Sandi Metz, Practical Object-Oriented Design, p44

## Pillars of OOP

"These terms can be expressed by the abbreviation of **abstraction, polymorphism, inheritance, and encapsulation (APIE)**. The letters APIE indicate the four basic pillars of OOP languages".

Miroslav Wengner, Practical Design Patterns for Java Developers, p6

### Abstraction

"Standard features"

Miroslav Wengner, Practical Design Patterns for Java Developers, p13

#### Not being able to identify an abstraction

"If you cannot correctly identify the abstraction, there may not be one, and if no common abstraction exists, then inheritance is not the solution to your design problem."

Sandi Metz, Practical Object-Oriented Design, p159

### Polymorphism

"Behaviour on demand"

Miroslav Wengner, Practical Design Patterns for Java Developers, p7

#### Polymorphism: Alternate definition

"Polymorphism in OOP refers to the ability of many different objects to respond to the same message. Senders of the message need not care about the class of the receiver; receivers supply their own specific version of the behavior."

Sandi Metz, Practical Object-Oriented Design, p94-95

#### Inheritance

"[...] the ability to create a new class above the existing subclass."

Miroslav Wengner, Practical Design Patterns for Java Developers, p7

##### Inheritance is Delegation

"Inheritances provides a way to define two objects as having a relationship such that when the first receives a message that it does not understand, it _automatically_ forwards, or delegates, the message to the second."

Sandi Metz, Practical Object-Oriented Design, p112

##### When to use inheritance

"[...] an object that uses a variable with a name like type or category to determine what message to send to self contains two highly related but slightly different types."

Sandi Metz, Practical Object-Oriented Design, p158

##### Difficulties of Inheritance

"Many of the difficulties of inheritance are caused by a failure to rigorously separate the concrete from the abstract."

Sandi Metz, Practical Object-Oriented Design, p122

##### Dynamic Binding

"... allows us to invoke methods on members of a class hierarchy without knowing what kind of specific object we are dealing with"

Object-Oriented Analysis, Design and Implementation, p62

##### Implementing an interface is a form of inheritance

"it should be pointed out that implementing the interface can also be viewed as a form of inheritance, where the implementing class inherits an abstract set of properties from the interface."

Object-Oriented Analysis, Design and Implementation, p58

##### Classes vs Interfaces

"In a way, classes and interfaces represent the extreme ends of a spectrum of possible implementations. When we write a class, we code every field and method; in other words, the code is complete in a sense. Interfaces are merely specifications."

Object-Oriented Analysis, Design and Implementation, p35

##### Good Hierarchies lead to the open-closed principle

"Use of inheritance results in cod that can be described as _open-closed_; hierarchies are open for extension while remaining closed for modification. Adding a new subclass to an existing hierarchy requires no changes to existing code. Hierarchies are thus _usable_; you can easily create new subclasses to accommodate new variants."

Sandi Metz, Practical Object-Oriented Design, p186

(See: [[SOLID#Open-Closed principle]] for reference)

##### Method Overloading

"This type is known as static polymorphism."

Miroslav Wengner, Practical Design Patterns for Java Developers, p8

##### Method Overriding

"This is sometimes called dynamic polymorphism."

Miroslav Wengner, Practical Design Patterns for Java Developers, p8

#### Mixins

"Many object-oriented languages provide a way to define a named group of methods that are independent of class and can be mixed in to any object."

Sandi Metz, Practical Object-Oriented Design, p143

#### Duck Typing

##### What are duck types

"Duck types are public interfaces that are not tied to any specific class."

Sandi Metz, Practical Object-Oriented Design, p85

##### Duck Types are Roles

"Role are names for _duck types_, simple interfaces that are not tied to any specific class and which are implemented by any object which responds to the right set of messages."

Avdi Grimm, Confident Ruby, p30

##### Duck Typing is about behavior

"It's not what an object _is_ what matters, it's what it _does_."

Sandi Metz, Practical Object-Oriented Design, p86

##### Duck Typing Benefit: Extensibility

"The final, duck typed, alternative is more abstract; it places slightly greater demands on your understanding but in return offers ease of extension."

Sandi Metz, Practical Object-Oriented Design, p94

### Encapsulation

"Encapsulation, which means that the module hides details of its implementation from external agents"

Object-Oriented Analysis, Design and Implementation, p7

#### Encapsulation: Alternate Definition

"Encapsulation is exposing only what's required"

(source?)

#### General Principle of Encapsulation

"This is the general principle of encapsulation. The state of an instance can be changed or updated through exposed methods or fields; everything else is hidden from the outside world."

Miroslav Wengner, Practical Design Patterns for Java Developers, p7

##### Always Hide Data

"[...] you should hide data from yourself. Doing so protects the code from being affected by unexpected changes. Data very often has behavior that you don't yet know about. Send messages to access variables, even if you think of them as data."

Sandi Metz, Practical Object-Oriented Design, p27

#### Law of inversion

"If your routines exchange too many data, put your routines in your data."

Brahma Dathan, Sarnath Ramnath, Object-Oriented Analysis, Design and Implementation, p206

## Coupling

"Low coupling allows us to modify a module without worrying about the ramifications of the changes on the rest of the system. By contrast, high coupling means that changes in one module would necessitate changes in other modules, which my have a domino effect and also make it harder to understand the code."

Object-Oriented Analysis, Design and Implementation, p8

## Cohesion

"Cohesion is a measure of how focused the responsibilities of a module are. If the responsibilities of a module are unrelated or varied and use different sets of data, cohesion is reduced."

Object-Oriented Analysis, Design and Implementation, p7d

### High Cohesion is having a single responsibility

"When everything in a class is related to its central purpose, the class is said to be _highly cohesive_ or to have a single responsibility."

Sandi Metz, Practical Object-Oriented Design, p22

(See [[SOLID#Single responsibility principle]] for reference)

## Association

"An association implies that an object of one class is making use of an object of another class and is indicated simply by a solid line connecting the two class icons."

Object-Oriented Analysis, Design and Implementation, p50

## Composition

### Message delegation is a consequence of composition

"Composition allows objects to have structural independence, but at the cost of explicit message delegation."

Sandi Metz, Practical Object Oriented-Design, p186
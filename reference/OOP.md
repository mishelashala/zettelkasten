## What is an object

"Each component *(object)* represents a data abstraction and is designed to store information along with procedures to manipulate the same"

Object-Oriented Analysis, Design and Implementation, p5.

## What is a software system

"The overall philosophy here is to define a software system as a collection of objects of various types that interact with each other through well-defined interfaces."

Object-Oriented Analysis, Design and Implementation, p5.

## Software Adaptability

"The ability to change the functionality of a component allows for systems to be more adaptable"

Object-Oriented Analysis, Design and Implementation, p8

## Pillars of OOP

"These terms can be expressed by the abbreviation of **abstraction, polymorphism, inheritance, and encapsulation (APIE)**. The letters APIE indicate the four basic pillars of OOP languages".

Miroslav Wengner, Practical Design Patterns for Java Developers, p6

## Distinctive characteristic of OOP

"What characterizes an object-oriented system is its ability to treat data and behavior as closely related."

Davi Vieira, Designing Hexagonal Architecture, p90

## OOP is about messages

"More than classes, inheritance, or encapsulation, the fundamental feature of an object oriented program is the sending of messages. Every action the program performs boils down to a series of messages sent to objects."

Avdi Grimm, Confident Ruby, p26

## OOP systems are defined by their messages

"[...] an object oriented application is more than just classes. It is made up of classes but _defined_ by messages."

Sandi Metz, Practical Object Oriented Design, p61

## Encapsulation

"Encapsulation, which means that the module hides details of its implementation from external agents"

Object-Oriented Analysis, Design and Implementation, p7

### Law of inversion

"If your routines exchange too many data, put your routines in your data."

Brahma Dathan, Sarnath Ramnath, Object-Oriented Analysis, Design and Implementation, p206

## What is coupling

"Low coupling allows us to modify a module without worrying about the ramifications of the changes on the rest of the system. By contrast, high coupling means that changes in one module would necessitate changes in other modules, which my have a domino effect and also make it harder to understand the code."

Object-Oriented Analysis, Design and Implementation, p8

## What is cohesion

"Cohesion is a measure of how focused the responsibilities of a module are. If the responsibilities of a module are unrelated or varied and use different sets of data, cohesion is reduced."

Object-Oriented Analysis, Design and Implementation, p7d

## What is association

"An association implies that an object of one class is making use of an object of another class and is indicated simply by a solid line connecting the two class icons."

Object-Oriented Analysis, Design and Implementation, p50

## Inheritance

### When to use inheritance

"[...] an object that uses a variable with a name like type or category to determine what message to send to self contains two highly related but slightly different types."

Sandi Metz, Practical Object-Oriented Design, p158

### Dynamic Binding

"... allows us to invoke methods on members of a class hierarchy without knowing what kind of specific object we are dealing with"

Object-Oriented Analysis, Design and Implementation, p62

### Implementing an interface is a form of inheritance

"it should be pointed out that implementing the interface can also be viewed as a form of inheritance, where the implementing class inherits an abstract set of properties from the interface."

Object-Oriented Analysis, Design and Implementation, p58

## Classes vs Interfaces

"In a way, classes and interfaces represent the extreme ends of a spectrum of possible implementations. When we write a class, we code every field and method; in other words, the code is complete in a sense. Interfaces are merely specifications."

Object-Oriented Analysis, Design and Implementation, p35
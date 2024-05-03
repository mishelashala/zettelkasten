# What application design is about

"_Application design is about changeability, not locking down the right design._"

Chris Sterling, Managing Software Design Debt, p154

# Design is an art

"Design is not an assembly line where similarly trained workers construct identical widgets; it's a studio where like-minded artists sculpt custom applications. Design is thus an art, the art of arranging code."

Sandi Metz, Practical Object-Oriented Design, p3

# Design is a process

"Design is a process of progressive discovery that relies on a feedback loop."

Sandi Metz, Practical Object-Oriented Design, p7

# Start of the design journey

"The design journey does not start in the code but by seeking business knowledge."

Davi Vieira, Designin Hexagonal Architectures, p387

# Ignoring previous knowledge

"We always have the prerogative to do things in our way, sometimes ignoring the knowledge resulting from the experience of others who came before us."

Designing Hexagonal Architecture with Java, p46

## BDUF is used to mitigate risk

"The reason for specifying business requirements and technical design before construction is to reduce risk."

Christ Sterling, Managing Software Debt, pxxiv

## Long feedback cycles produce BDUFs

"Generally, these problems with BDUF are symptoms of feedback cycles that are too long in duration."

Christ Sterling, Managing Software Debt, ppxxv

## Late integration

"The longer the wait to integrate, the more difficulties arise when generating a stabilized build of an application."

Chris Sterling, Managing Software Debt, p8

# Postpone Decisions

"Because you are writing changeable code, you are best served by postponing decisions until you are absolutely forced to make them."

Sandi Metz, Practical Object-Oriented Design, p32

## When to postpone a decision

"When the future cost of doing nothing is the same as the current cost, postpone the decision."

Sandi Metz, Practical Object-Oriented Design, p23

## Who should make application design decisions

"Those who are closes to the implementation details, with external support as necessary, should make application design decisions."

Chris Sterling, Managing Software Debt, p154

# The problem with poorly designed small applications

"The problem with poorly designed small applications is that if they are successful, they grow up to be poorly designed big applications."

Sandi Metz, Practical Object-Oriented Design, p3

# Big Ball of Mud

"A BIG BALL OF MUD is a casually, even haphazardly, structured system. Its organization, if one can call it that, is dictated more by expediency than design.""

Brain Foot and Joseph Yoder, www.laputan.org/mud/mud.html.

# Refactoring Reveals design

"Do these refactorings even when you do not know the ultimate design. They are needed, not because the design is clear, but because it isn't. You do not have to know where you're going to use good design practices to get there. Good practices reveal good design."

Sandi Metz, Practical Object-Oriented Design, p31

## What is code design

"Every application is a collection of code; the code's arrangement is the design."

Sandi Metz, Practical Object-Oriented Design, p3

### Practical code design

"Practical Design does not anticipate what will happen to your application; it merely accepts that something will and that, in the present, you cannot know what."

Sandi Metz, Practical Object-Oriented Design, p4

### Why code must be easy to change

"To efficiently evolve, code must be easy to change."

Sandi Metz, Practical Object-Oriented Design, p22

### Definition of Code Easy to change

- changes have no unexpected side effects,
- small changes in requirements require correspondingly small changes in code,
- existing code is easy to reuse, and
- the easiest way to make a change is to add code that in itself is easy to change

Sandi Metz, Practical Object-Oriented Design, p16

### The craft of programming

"Your application needs to work right now just once; it must be easy to change forever. This quality of easy changeability reveals the craft of programming."

Sandi Metz, Practical Object-Oriented Design, p15

### Good code is a matter of arrangement style

"Early OO programmers noticed that some code arrangements made their lives easier while other made them harder. These experiences led them to develop opinions about how to write good code."

Sandi Metz, Practical Object-Oriented Design, p5

## Good Code is TRUE

"Code that is Transparent, Reasonable, Usable, and Exemplary (TRUE) not only meets today's needs but can also be change to meet the needs of the future."

Sandi Metz, Practical Object-Oriented Design, p17

### TRUE Acronym

- Transparent: The consequences of change should be obvious in the code that is changing and in distant code that relies upon it.
- Reasonable: The cost of any change should be proportional to the benefits the change achieves.
- Usable: Existing code should be usable in new and unexpected contexts.
- Exemplary: The code itself should encourage those who change it to perpetuate these qualities.

Sandi Metz, Practical Object-Oriented Design, p16-17

## Law of Demeter

### Definition
"Demeter is often paraphrased as 'only talk to your immediate neighbors' or 'use only one dot'."

Sandi Metz, Practical Object-Oriented Design, p81

### Wrapper methods to enforce the Demeter law

"One common way to remove train wrecks from code is to use delegation to avoid dots. In object-oriented terms, to _delegate_ a message is to pass it on to another object, often via a wrapper method. The wrapper method encapsulates, or hides, knowledge that would otherwise be embodied in the message chain."

Sand Metz, Practical Object-Oriented Design, p82

### Demeter violations are signals of an API lacking behavior

```ts
// train wreck
api
	.doThis()
	.doThat()
	.and()
	.that()
```

"The train wrecks of Demeter violations are clues that there are objects whose public interfaces are lacking. Listening to Demeter means paying attention to your point of view. If you shift to a message-based perspective, the messages you find will become public interfaces in the objects they lead you to discover."

Sandi Metz, Practical Object-Oriented Design, p83

### Message chaining breaks the law of demeter

"Message chaining creates a dependency between the original object and every object and message along the way to its ultimate target. These additional couplings greatly increase the chance that the first object will be forced to change because a change to _any_ of the intermediate objects might affect it."

Sandi Metz, Practical Object-Oriented Design, p40

## The problem with ORMs

"[...] if we combine an ORM framework with a layered architecture, we're easily tempted to mix business rules with persistence aspects."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p11

## Handling Exceptions

"One of the characteristics of a well-designed software system is that it appropriately uses exceptions to handle unexpected situations."

Object-Oriented Analysis, Design and Implementation, p81
## Start of the design journey

"The design journey does not start in the code but by seeking business knowledge."

Davi Vieira, Designin Hexagonal Architectures, p387

## BDUF is used to mitigate risk

"The reason for specifying business requirements and technical design before construction is to reduce risk."

Christ Sterling, Managing Software Debt, pxxiv

## Long feedback cycles produce BDUFs

"Generally, these problems with BDUF are symptoms of feedback cycles that are too long in duration."

Christ Sterling, Managing Software Debt, ppxxv

## Late integration

"The longer the wait to integrate, the more difficulties arise when generating a stabilized build of an application."

Chris Sterling, Managing Software Debt, p8

## When to postpone a decision

"When the future cost of doing nothing is the same as the current cost, postpone the decision."

Sandi Metz, Practical Object-Oriented Design, p23

## Who should make application design decisions

"Those who are closes to the implementation details, with external support as necessary, should make application design decisions."

Chris Sterling, Managing Software Debt, p154

## What is code design

"Every application is a collection of code; the code's arrangement is the design."

Sandi Metz, Practical Object-Oriented Design, p3

### Practical code design

"Practical Design does not anticipate what will happen to your application; it merely accepts that something will and that, in the present, you cannot know what."

Sandi Metz, Practical Object-Oriented Design, p4

### Why code must be easy to change

"To efficiently evolve, code must be easy to change."

Sandi Metz, Practical Object-Oriented Design, p22

## Law of Demeter

### Definition
"Demeter is often paraphrased as 'only talk to your immediate neighbors' or 'use only one dot'."

Sandi Metz, Practical Object-Oriented Design, p81

### Wrapper methods to enforce the Demeter law

"One common way to remove train wrecks from code is to use delegation to avoid dots. In object-oriented terms, to _delegate_ a message is to pass it on to another object, often via a wrapper method. The wrapper method encapsulates, or hides, knowledge that would otherwise be embodied in the message chain."

Sand Metz, Practical Object-Oriented Design, p82

## The problem with ORMs

"[...] if we combine an ORM framework with a layered architecture, we're easily tempted to mix business rules with persistence aspects."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p11

## Handling Exceptions

"One of the characteristics of a well-designed software system is that it appropriately uses exceptions to handle unexpected situations."

Object-Oriented Analysis, Design and Implementation, p81
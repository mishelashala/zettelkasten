#DDD 

## Entity

"What characterizes an entity is its sense of continuity and identity."

Designing Hexagonal Architecture with Java, p15

### Domain Entity Purity

"Domain entities should be pure in the sense that they deal only with business concerns."

Designing Hexagonal Architecture with Java, p29

#### Benefit

[[Hexagonal Architecture#Pure Domain equals Change Tolerant Design]]

Davi Vieira, Designin Hexagonal Architectures, p386

### Domain Integrity

#### When validations are not feasible in the entity

"If it's not feasible to validate a business rule in a domain entity, we can do it in the use case code before it starts working on the domain entities."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p43

---

## Value Objects

"Value objects help us complement our code's expressiveness when there is no need to identify something uniquely, as well as when we are more concerned about the object's attributes than its identity."

Designing Hexagonal Architecture with Java, p16

---

## Policies

"A policy, also known as a strategy, is a pattern that encapsulates part of the problem domain in a block of code."

Designing Hexagonal Architecture with Java, p47

---

## Knowledge Crunching

"Knowledge Crunching is based on brainstorming between [...] developers and domain experts."

Designing Hexagonal Architecture with Java, p28

---

## Domain Model

### Domain Model is a subproduct

"The domain model is the outcome of people trying to understand the business and translating that understanding into code."

Davi Vieira, Designin Hexagonal Architectures, p391

### Pure Domain Model

"[...] the code that does not merge business concerns with technology ones"

Davi Vieira, Designin Hexagonal Architectures, p386

### Rich Domain Model

"In a rich domain model, as much of the domain logic as possible is implemented within the entities at the core of the application. The entities provide methods to change the state and only allow changes that are valid according to the business rules."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p44

### Anemic Domain Model

"The entity objects coming from anemic domain models generally have data but lack behavior."

Designing Hexagonal Architecture with Java, p30

"In an 'anemic' domain model, the entities themselves are very thin. They usually only provide fields to hold the state and getter and setter methods to read and change the state. They don't contain any domain logic."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p44

#### Downside of an anemic domain model

"When behavior is not present on domain objects, we have to go somewhere else to fully grasp what the entity is supposed to do, thus generating a mental overload that can quickly become an onerous burden as the code base grows."

Designing Hexagonal Architecture with Java, p30

### Domain Model with Mixed Concerns

"If we blend primary and secondary activities, we'll end up with a domain model with mixed concerns."

Davi Vieira, Designin Hexagonal Architectures, p392

---

## Subdomain

"The purpose of a subdomain is to group the elements that support the core domain but cannot be considered elements that express the core domain."

Davi Vieira, Designin Hexagonal Architectures, p392

---

## Bounded Contexts

### Communication Between Bounded Contexts

"If one context needs something of the other, they can call each other's domain services, or we can introduce an application service as a coordinator between the bounded contexts."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p60

---

## Transactions

### Transaction Boundary

"A transaction should span all write operations to the database that are performed within a certain case, ensuring that all those operations can be rolled back together if one of them fails."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p66
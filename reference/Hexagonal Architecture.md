## Goal

"One of the hexagonal architecture's ultimate goals is to allow developers to test the application when its external dependencies are not present, such as its UI and databases."

Designing Hexagonal Architecture with Java, p 25

## Driven Operations

"These operations are triggered from your application and go into the outside world to get data to fulfill the software's needs. A drive operation generally occurs in response to some driving one."

Designing Hexagonal Architecture with Java, p21

### Most Common Driven Operations

"Driven operations baed on data persistence are the most common."

Davi Vieira, Designing Hexagonal Architecture, p137

## Driving Operations

"Driving operations are the ones that request actions to the software."

Designing Hexagonal Architecture with Java, p20

### Why driving operations are named like that

"Through the lens of the hexagonal architecture, the input side of a system is controlled by driving operations. We call them driving operations because they actually initiate and drive the behavior of a hexagonal application."

Davi Vieira, Designing Hexagonal Architecture

### System Under Discussion Actors

"We can classify the SuD actors: the driver actor is a person or system that triggers one of the SuD behaviors, while the driven actor is an external system consumed by the SuD."

Designing Hexagonal Architecture with Java, p60

## Adapters

### The role of adapters

"We use adapters to allow a system to be compatible with different technologies or protocols."

Designing Hexagonal Architecture with Java, p78

### Advantages

"What is so compelling about the hexagonal architecture is that we can add and remove adapters without worrying about changing the core system logic wrapped in the domain hexagons."

Davi Vieira, Designin Hexagonal Architectures, p226

### Input Adapters

#### Input adapters and primary actors

"The interaction between primary actors and the hexagonal application occurs through input adapters. Such interaction is defined by driving operations."

Designing Hexagonal Architecture with Java, p80

#### The role of input adapters

"When building the application hexagon, we need to create use cases and input ports to express system capabilities. To make these capabilities available to users and other systems, we need to build input adapters and connect them to input ports."

Davi Vieira, Designin Hexagonal Architectures, p233

#### Input adapters as protocols

"[...] input adapters work like protocols, defining which technologies are supported as a menas to access the features provided by a hexagonal system. Input adapters mark a clear frontier between with is inside the hexagonal and what is outside, and perform what we call driving operations."

Designing Hexagonal Architecture with Java, p80

### Output Adapters

#### Output adapter's role

"The output adapter's role in the hexagonal architecture is to deal with drive operations."

Davi Vieira, Designing Hexagonal Architecture, p91

### Output Port

#### Output port's goal

"The output port's main goal is to state what kind of data it needs without specifying how it will get that data. That's why we define them as interfaces and not implementations."

Designing Hexagonal Architecture with Java, p73

#### Output Adapter Mapping Flow

"When building a web adapter to an application, we should keep in mind that we're building an adapter that translates HTTP protocol to method calls on the use cases of our application, translates the results back to HHTP, and does not do any domain logic."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p54

#### Why use output ports

"The reason to create and utilize output ports will be derived from the activities performed by use cases."

(Source?)

### Persistance Adapter

"[...] the persistence adapter is a driven or outgoing adapter because it's called by our application and not the other way around."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p56

#### Benefit

"Building a persistence adapter that acts as a plugin to the domain code frees the domain code from persistence details so that we can build a rich domain model."

Tom Hombergs, Get Your Hands Dirty on Clean 
Architecture, p66

## Distributed Hexagonal Architecture

"In a distributed approach, two or more hexagonal self-contained systems can comprise the whole hexagon-based system."

Davi Vieira, Designing Hexagonal Architecture, p134

## Why separate the domain layer from the application layer

"Our intention at the highest level is to validate business ideas straight on the Domain hexagon without the aid of things present on Application and Framework hexagon."

Davi Vieira, Designin Hexagonal Architecture, p160

### Application layer should not know about HTTP

"If the application core knowns that we're dealing with HTTP on the outside, we have lost the option to perform the same domain logic from other incoming adapters that do not use HTTP."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p50

### Outer layers are technology-specific

"As things move on to these hexagons, they tend to become more technology-specific, operating at a lower level, because technology-specific things are far away from the Domain hexagon."

Davi Vieira, Designin Hexagonal Architecture, p160

### Pure Domain equals Change Tolerant Design

"As long as you keep the code in the Domain hexagon that purely expresses the problem domain [...] you are on the right path to ensuring the encapsulation level that favors a more change-tolerant design."

Davi Vieira, Designin Hexagonal Architectures, p386

### Benefit of decoupling domain and infrastructure

"The domain code is free to be modeled as best fits the business problems, while the persistence and UI code are free to be modeled as best fits the persistence and UI problems."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p24

## Directory Structure

"The package boundaries, combined with package-private visibility, enable us to avoid unwanted dependencies between features."

Tom Hombergs, Get Your Hands Dirty on Clean Architecture, p27

## Hexagonal Architectural and DDD

"An always-present concern to separate what constitutes the core problem domain and what is secondary to it makes DDD a suitable approach to support the hexagonal architecture goal to separate technology code from business code."

Designing Hexagonal Architecture with Java, p27

### Entities in an Hexagonal Architecture

"Entities are first-class citizens in a hexagonal architecture. They are the foundational elements from which other software component will derive. But they alone aren't enough to create rich domain models, because not everything in a domain possesses an identity."

Designing Hexagonal Architecture with Java, p34
## Definition

"Technical debt is the decay of component and inter-component behavior when the application functionality meets a minimum standard of satisfaction for its users."

Chris Sterling, Managing Software Debt, p18

## Downsides of tech debt

### Software Debt makes adding new features harder

"As software debt grows in an application, the increased cost of delivery will eventually overtake the value realized by implementing new features."

Chris Sterling, Managing Software Debt, p5

### Tech debt decreases confidence

"As technical debt increases in your software, the confidence with which team members approach the code decreases."

Chris Sterling, Managing Software Debt, p24-25

## How Technical Debt is Acquired

"These are the activities that a team or team members choose not to do well now and will impede future development if left undone."

Chris Sterling, Managing Software Debt, p3

## How software debt accumulates

"Software debt accumulates when the focus is on immediate completion and changeability is neglected."

Chris Sterling, Managing Software Debt, p2

### Schedule Pressure causes tech debt

"When teams are held to a commitment that is unreasonable, they are bound to cut corners in order to meet the expectations of management."

Chris Sterling, Managing Software Debt, p19

### Lack of experience

"If a team lacks the ability and experience to identify when they are putting technical debt into software, it will be difficult to avoid adding technical debt."

Chris Sterling, Managing Software Debt, p17

#### Lack of Expertise is a liability

"An indicator of a software asset liability is when there is limited expertise available to work on an application."

Chris Sterling, Managing Software Debt, p8

#### The problem with limited expertise availability

"If the skills to work on the software are scarce in the industry, it is likely that the cost for someone with those skills is much higher than for people with more common skills."

Chris Sterling, Managing Software Debt, p8

### Moral Hazard

"Moral hazard is the view that parties insulated from risk may behave differently from the way they would behave if they were fully exposed to the risk."

Chris Sterling, Managing Software Debt

## What happens when software debt accumulates

"At some point small forms of decay in software become large enough to affect delivery to a point where working harder and longer doesn't result in successful outcomes."

Chris Sterling, Managing Software Debt, p2

## Tech debt is not free

"[...] short-term technical debt comes with consequences. Teams that take on technical debt often or in large doses are challenged with potentially dire consequences to the sustainability of their software."

Chris Sterling, Managing Software Debt, p13

## Remove tech debt asap

"The longer an instance of technical debt exists in the code, the more code will surround and interact with it, thus making the debt more difficult to remove."

Chris Sterling, Managing Software Debt, p23

## Pay tech debt immediately

"Paying off technical debt immediately goes agains the software industry project norms. Teams are used to coding only the feature they are currently working on and leaving technical improvements for a later time, even though later never seems to arrive."

Chris Sterling, Managing Software Debt, p23

## The cost of addressing technical debt increases with time

"No matter what, the cost of addressing technical debt increases with time."

Chris Sterling, Managing Software Debt, p20

## When is to late to pay software debt

"People involved in the project stay late working to get the release out the door. At this point it is too late to pay back the debt accrued during feature development."

Chris Sterling, Managing Software Debt, p2

## How to address tech debt

"The first step in addressing technical debt is acknowledging that it exists and is detrimental to the maintenance of the software you are working on."

Chris Sterling, Managing Software Debt, p23

### Strategies

#### Exceptions over comments

"Instead of using 'cleanup' comments, throw strategically placed runtime exceptions into the code so that it is left in a broken state. This way you will not be inclined to check in the code with the existing technical debt you know should be cleaned up."

Chris Sterling, Managing Software Debt, p26

### Feature Delivery vs Debt Reduction

"If software development teams and organizations are going to manage software debt, they must strike a balance between feature delivery for business gain and changeable software for the long haul."

Chris Sterling, Managing Software Debt, p13

## Why tech debt is ignored

"Because technical debt cannot be measured, business stakeholders and management easily ignore it."

Chris Sterling, Managing Software Debt, p17

## Types of debt

### Design Debt

"The cost of adding features is increasing toward the point where it is more than the cost of writing from scratch."

Chris Sterling, Managing Software Debt, p3

### Quality Debt

"There is a diminishing ability to verify the functional and technical quality of software."

Chris Sterling, Managing Software Debt, p3

#### Quality Debt Indicators

- Lengthening regression test execution
- Increasing known unresolved defects
- Creating a maintenance team for production issues

Cris Sterling, Managing Software Debt, p85

### Platform Experience Debt

"The availability of people to work on software changes is becoming limited or cost-prohibitive."

Chris Sterling, Managing Software Debt, p3

### Like-to-Like migration

"[...] teams and management start to discuss replacing [the system] with 'better' and 'newer' solution. This is sometimes called like-to-like migration, rewrite, system replacement, 'next gen' [...]."

Chris Sterling, Managing Software Debt, p6

#### Like-to-Like migrations are not copy + paste

"Once business sponsors are told about a like-to-like migration, they think that all the features can just be copied from the current version. Some stakeholders will have changes, additions, and updates."

Chris Sterling, Managing Software Debt, p7

#### Like-to-like migrations take longer

"Like-to-like migrations always take longer than expected and therefore are surprisingly costly. Customers become frustrated with the amount of time taken to develop the migrated version of the application."

Chris Sterling, Managing Software Debt, p7

## Software Defect

"Defects are system faults that users are able to work around but should not occur in a functioning software implementation."

Christ Sterling, Managing Software Debt, p50

## Software Fires

"Fires are defects that cannot be worked around and cause serious problems for users of the software."

Chris Sterling, Managing Software Debt, p50-51

## Quality as an after thought

### The result of quality as an after thought

"[...] afterthought result in debt. Over time this debt becomes too costly to even think of paying back, [...]"

Chris Sterling, Managing Software Debt, p82

## Practices to sustain internal quality

- Sustainable pace
- Early identification of internal quality problems
- Close Collaboration
- Refactoring
- Small batches of work
- Defining technically done
- Potentially shippable product increments
- Single work queue

Chris Sterling, Managing Software Debt

## Late Integration

### Problems caused by integrating late

"Problems that were introduced earlier in development emerge during integration, such as duplicate code, merge conflicts, incompatible interfaces, and misaligned feature interpretations."

Chris Sterling, Managing Software Debt, p8

## Tracer Bullet

"Tracer bullet: a narrow implementation in production quality of a large feature to be implemented into the product later that will enable the team to better estimate the remaining feature work"

Chris Sterling, Managing Software Debt, p192

### Tracer Bullet Usage

"If your target is moving, or if you don't know all the factors, you use tracer bullets--little phosphorous rounds intermixed with real rounds in your gun. As you fire, you can actually see the traer bullets. And where they are landing is where the actual bullets are landing. I you're not quite on target--because you can see if you're not on target--you can adjust your position."

> Note: secondary source.
> Original source: "Tracer Bullets and Prototypes: A conversation with Andy Hunt and Dave Thomas, part VIII"

Chris Sterling, Managing Software Debt, p195

## Technology Research

"Research: broad, foundational gaining of knowledge to decide what to spike or to obtain the ability to estimate features desired in the future"

Chris Sterling, Managing Software Debt, p192

## Technology Spike

"Spike: a quick and dirty implementation, design to be thrown away, to gain knowledge about a larger feature or integrating technology"

Chris Sterling, Managing Software Debt, p192

## SAID Acronym

1. Structure: how the pieces (components) create a solution (application).
2. Alignment: the degree to which the application or enterprise structure align to current business objectives and strategy.
3. Integrity: the components that provide stability to the structure (application or enterprise)
4. Design: a way to conceptually communicate the planned or implemented structure of a component, application, or enterprise.

Chris Sterling, Managing Software Debt, p178
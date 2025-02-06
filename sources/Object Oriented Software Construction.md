Bertrand Meyer,  
Interactive Software Engineering Inc. (ISE) 270 Storke Road, Suite 7  
Santa Barbara, CA 93117  
USA  
805-685-1006, fax 805-685-6869 <meyer@tools.com>, http://www.tools.com

## Notes

### External Quality Factors

«such qualities as speed or ease of use, whose presence or absence in software product may be detected by its users. These properties may be called **external** quality factors.», p3

### Internal Quality Factors

«Other qualities applicable to a software product, such as being modular, or readable, are **internal** factors, perceptible only to computer professionals who have access to the actual software text.», p3

### Internal vs External Quality Factors

«the key to achieving these external factors is in the internal ones: for the user to enjoy the visible qualities, the designers and implementers must have applied internal techniques that will ensure the hidden qualities.», p3

### Not loosing the big picture

«We should not, however, lose track of the global picture; the internal techniques are not an end in themselves, but a means to reach external software qualities.», p4

### Definition of Correctness

«Correctness is the ability of software products to perform their exact tasks, as defined by their specification.», p4

### The Importances of correctness

«Correctness is the prime quality. If a system does not do what it is supposed to do, everything else about it — whether it is fast, has a nice user interface... — matters little.», p4

### To achieve correctness is hard

«Even the first step to correctness is already difficult: we must be able to specify the system requirements in a precise form, by itself quite a challenging task.», p4

### Conditional Correctness

«In the conditional approach to correctness, we only worry about guaranteeing that each layer is correct _on the assumption_ that the lower levels are correct.», p4

### Why rely on conditional correctness

«it achieves separation of concerns and let us concentrate at each stage on a limited set of problems.», p4

### Definition of Robustness

«Robustness is the ability of software systems to react appropriately to abnormal conditions.», p5

### Correctness and Robustness complement each other

«Correctness addresses the behavior of a system in cases covered by its specification; robustness characterizes what happens outside of that specification.», p5

### Abnormal cases

«an abnormal case is simply a case that is not covered by the specification.», p6

### Widening the specification

«If you widen the specification, cases that used to be abnormal become normal—even if they correspond to events such as erroneous user input that you would prefer not to happen.», p6

### Normal cases

«"Normal" in this sense does not mean "desirable", but simply "planned for in the design of the software".», p6

### The point of robustness in the face of abnormal cases

«There will always be cases that the specification does not explicitly address. The role of the robustness requirement is to make sure that if such cases do arise, the system does not cause catastrophic events», p6

### Definition of Extensiblity

«Extensibility is the ease of adapting software products to changes of specification.», p6

### Extensibility is a matter of scale

«For small programs change is usually not a difficult issue; but as software grows bigger, it becomes harder and harder to adapt.», p7

### Traditional approaches to software development didn't had change in mind

«Traditional approaches to software engineering did not take enough account of change, relying instead on an ideal view of the software lifecycle where an initial analysis stage freezes the requirements, the rest of the process being devoted to designing and building a solution.», p6

### First essential principle to favor extensibility

«_Design simplicity_: a simple architecture will always be easier to adapt to changes than a complex one.», p7

### Second essential principle to favor extensibility

«_Decentralization_: the more autonomous the modules, the higher the likelihood that a simple change will affect just one module, or a small number of modules, rather than triggering off a chain reaction of changes over the whole system.», p7

### OOP is about simplicity and decentralization

«The object-oriented method is, before anything else, a system architecture method which helps designers produce systems whose structure remains both simple (even for large systems) and decentralized.», p7

### Definition of Reusability

«Reusability is the ability of software elements to serve for the construction of many different applications.», p8

### The need for reusability

«The need for reusability comes from the observation that software systems often follow similar patterns; it should be possible to exploit this commonality and avoid reinventing solutions to problems that have been encountered before. By capturing such a pattern, a reusable software element will be applicable to many different developments.», p7

### Why favor reusability

«solving the reusability problem essentially means that less software must be written, and hence that more effort may be devoted (for the same total cost) of improving the other factor,s such as correctness and robustness.», p7

### Definition of Compatibility

«Compatibility is the ease of combining software elements with others.», p8

### Why compatibility is important

«we do not develop software elements in a vacuum: they need to interact with each other.»

### What causes compatibility problems

«But they too often have trouble interacting because they make conflicting assumptions about the rest of the world.», p8

### Definition of Efficiency

«Efficiency is the ability for a software system to place as few demands as possible on hardware resources, such as processor time, space occupied in internal and external memories, bandwith used in communication devices.», p9

## Bibliography
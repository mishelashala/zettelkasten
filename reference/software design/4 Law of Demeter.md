#SoftwareLaws 

## Definition
"Demeter is often paraphrased as 'only talk to your immediate neighbors' or 'use only one dot'."

Sandi Metz, Practical Object-Oriented Design, p81

---

## Wrapper methods to enforce the Demeter law

"One common way to remove train wrecks from code is to use delegation to avoid dots. In object-oriented terms, to _delegate_ a message is to pass it on to another object, often via a wrapper method. The wrapper method encapsulates, or hides, knowledge that would otherwise be embodied in the message chain."

Sand Metz, Practical Object-Oriented Design, p82


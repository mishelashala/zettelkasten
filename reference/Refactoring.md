## Definition

"Refactoring is defined simply as the process of improving the internal structure (design and code) of a piece of software without altering the module's external behavior."

Brahma Dathan, Sarnath Ramnath, Object-Oriented Analysis, Design and Implementation, p199

## Boy Scout Rule

"Always leave the code in better shape than when you started."

Chris Sterling, Managing Software Debt, p63

## Refactoring List

### Extract Method Rule

"If you have a code fragment that can be grouped together, turn the fragment int on a method and assign it a name that explains the purpose of the method."

Brahma Dathan, Sarnath Ramnath, Object-Oriented Analysis, Design and Implementation, p205

### Move Method Rule

"If we have a method that is using more features of another class than the class on which it is defined, then the method needs to be moved to the class whose features it is using."

Brahma Dathan, Sarnath Ramnath, Object-Oriented Analysis, Design and Implementation, p207

## Refactoring Hierarchies

### General rule for refactoring hierarchies

"The general rule for refactoring into a new inheritance hierarchy is to arrange code so that you can promote abstractions rather than demote concretions."

Sandi Metz, Practical Object-Oriented Design, p123


## Problem Solving

### Formalize a problem before attempting to solve it

«once a problem is formalized, we can look for solutions in terms of a precise model and determine whether a program already exists to solve that problem.»

Alfred Aho, Data Structures and Algorithms

### Stepwise Refinement

«To convert such an informal algorithm to a program, however, we must go through several stages of formalization (called _stepwise refinement_) until we arrive at a program the meaning of whose steps are formally defined by a language manual.»

Alfred Aho, Data Structures and Algorithms

## Algorithms

### Definition of Algorithm

«a finite sequence of instructions, each of which has a clear meaning and can be performed with a finite amount of effort in a finite length of time»

Alfred Aho, Data Structures and Algorithms

### Algorithms can be executed any number of times

«In an algorithm instructions can be executed any number of times, provided the instructions themselves indicate repetition.»

Alfred Aho, Data Structures and Algorithms

### Algorithms must be finite

«no matter what the input values may be, an algorithm terminate after executing a finite number of instructions.»

Alfred Aho, Data Structures and Algorithms

### Heuristic Algorithm

«An algorithm that quickly produces good but not necessarily optimal solutions is called a _heuristic_»

Alfred Aho, Data Structures and Algorithms

## Algorithmic Design

### Goals of algorithm design

1. We would like an algorithm that is easy to understand, code, and debug.
2. We would like an algorithm that makes efficient use of the computer's resources, especially, one that runs as fast as possible.

Alfred Aho, Data Structures and Algorithms

### Running Time as a function of the input

«The fact that running time depends on the input tells us that the running time of a program should be fined as a function of the input. Often, the running time depends not on the exact input but only on the "size" of the input.»

Alfred Aho, Data Structures and Algorithms

## Graphs

### Definition of Graph

«A _graph_ consists of a set of points called _vertices_, and lines connecting the points, called _edges_.»

Alfred Aho, Data Structures and Algorithms

### Coloring of a Graph

«A _coloring_ of a graph is an assignment of a color to each vertex of the graph so that not two vertices connected by an edge have the same color.»

Alfred Aho, Data Structures and Algorithms

### Coloring and NP-Complete problems

«coloring an arbitrary graph with as few colors as possible is one of a large class of problems called "NP-complete problems," for which all known solutions are essentially of the type "try all possibilities."»

Alfred Aho, Data Structures and Algorithms

### Greedy Coloring Algorithm

«One reasonable heuristic for graph coloring is the following "greedy" algorithm. Initially we try to color as many vertices as possible with the first color, then as many as possible of the uncolored vertices with the second color, and so on.»

Alfred Aho, Data Structures and Algorithms

(See [[#Heuristic Algorithm]] for reference)

### k-clique definition

«In graph theory, a _k-clique_ is a set of _k_ vertices, every pair of which is connected by an edge.»

Alfred Aho, Data Structures and Algorithms

### k-color definition

«Obviously, _k_ colors are needed to color a _k_-clique, since no two vertices in a clique may be given the same color.»

Alfred Aho, Data Structures and Algorithms

## Procedures

### Definition

«Procedures, [...], generalize the notion of an operator.»

Alfred Aho, Data Structures and Algorithms

### Benefits of procedures

«by using procedures a programmer is free to define his own operators and apply them to operands that need not the basic types.»

Alfred Aho, Data Structures and Algorithms

### Another benefit of procedures

«Another advantage of procedures is that they can be used to encapsulate parts of an algorithm by localizing in one section of a program all the statements relevant to a certain aspect of a program.»

Alfred Aho, Data Structures and Algorithms

## Encapsulation

### Example

«An example of encapsulation is the use of one procedure to read all input and to check for its validity.»

Alfred Aho, Data Structures and Algorithms

## Abstract Data Types

### Definition

«An abstract data type is a mathematical model, together with various operations defined on the model.»

Alfred Aho, Data Structures and Algorithms

### How to represent ADTs in code

«To represent the mathematical model underlying and ADT we use _data structures_[[Data Structures#Data Structures]]».

Alfred Aho, Data Structures and Algorithms

## Data Structures

### Definition

«[Data Structures] are collections of variables, possibly of several different data types, connected in various ways.»

Alfred Aho, Data Structures and Algorithms

### Cell as the building block of data structures

«The _cell_ is the basic building block of data structures. We can picture a cell as a box that is capable of holding a value drawn from some basic or composite data type.»

Alfred Aho, Data Structures and Algorithms

### Data Structures are aggregates of named cells

«Data structures are created by giving names to aggregates of cells and (optionally) interpreting the values of some cell as representing connections (e.g., pointers) among cells.»

Alfred Aho, Data Structures and Algorithms

### Cell-Grouping

#### Array as the simplest aggregation mechanism

«The simplest aggregating mechanism in Pascal and most other programming languages is the (one-dimensional) array»

Alfred Aho, Data Structures and Algorithms

##### Array: Definition

«[An array] is a sequence of cells of a given type, which we shall often refer to as the cell type.»

Alfred Aho, Data Structures and Algorithms

#### Records as a common grouping mechanism

«Another common mechanism for grouping cells in programming languages is the _record structure_.»

Alfred Aho, Data Structures and Algorithms

##### Record Structure: Definition

«A _record_ is a cell that is made up of a collection of cells, called _fields_, of possibly dissimilar types.»

Alfred Aho, Data Structures and Algorithms

### Pointers and cursors as an alternative to cell-grouping

«In addition to the cell-grouping features of a programming language, we can represent relationships between cells using points and cursors.»

Alfred Aho, Data Structures and Algorithms

#### Pointer: Definition

«A _pointer_ is a cell whose value indicates another cell.»

Alfred Aho, Data Structures and Algorithms

##### How do we represent graphically pointers

«When we draw pictures of data structures, we indicate the fact that cell _A_ is a pointer to cell _B_ by drawing an arrow from _A_ to _B_.»

Alfred Aho, Data Structures and Algorithms

#### Cursor: Definition

«A _cursor_ is an integer-valued cell, used as a pointer to an array.»

Alfred Aho, Data Structures and Algorithms

#### Cursors are pointers

«As a method of connection, the cursor is essentially the same as a pointer.»

Alfred Aho, Data Structures and Algorithms
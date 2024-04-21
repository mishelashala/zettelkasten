# Definition of Algorithm

«a finite sequence of instructions, each of which has a clear meaning and can be performed with a finite amount of effort in a finite length of time»

Alfred Aho, Data Structures and Algorithms

## Algorithms can be executed any number of times

«In an algorithm instructions can be executed any number of times, provided the instructions themselves indicate repetition.»

Alfred Aho, Data Structures and Algorithms

## Algorithms must be finite

«no matter what the input values may be, an algorithm terminate after executing a finite number of instructions.»

Alfred Aho, Data Structures and Algorithms

## Heuristic Algorithm

«An algorithm that quickly produces good but not necessarily optimal solutions is called a _heuristic_»

Alfred Aho, Data Structures and Algorithms

# Goals of algorithm design

1. We would like an algorithm that is easy to understand, code, and debug.
2. We would like an algorithm that makes efficient use of the computer's resources, especially, one that runs as fast as possible.

Alfred Aho, Data Structures and Algorithms

# Running Time

## Running Time as a function of the input

«The fact that running time depends on the input tells us that the running time of a program should be fined as a function of the input. Often, the running time depends not on the exact input but only on the "size" of the input.»

Alfred Aho, Data Structures and Algorithms

### Running time as a function of the input type

«For many programs, the running time is really a function of the particular input, and not just the input size.»

Alfred Aho, Data Structures and Algorithms

### Running time notation

«It is customary, then, to talk of _T(n)_, the running time of program on inputs of size _n_. For example, some program may have a running time of _T(n) = cn^2_, where _c_ is a constant.»

Alfred Aho, Data Structures and Algorithms

### We cannot represent running time in seconds

«the running time of a program depends on the compiler used to compile the program and the machine used to execute it. These facts imply that we cannot express the running time _T(n)_ in standard time units such as seconds.»

Alfred Aho, Data Structures and Algorithms

### Units of running time are unspecified

«The units of _T(n)_ will be left unspecified, but we can think of _T(n)_ as being the number of instructions executed on an idealized computer.»

Alfred Aho, Data Structures and Algorithms

### Running time as the product of a growth rate function

«We say that _T(n)_ is _O(f(n))_ if there are constants _c_ and _n0_ such that _T(n) <= cf(n)_ whenever _n >= n0_. A program whose running time is _O(f(n))_ is said to have _growth rate f(n)_.»

Alfred Aho, Data Structures and Algorithms

## Growth rates

«To talk about growth rates of functions we use what is known as "big-oh" notation. [..] When we say the running time _T(n)_ of some program is _O(n^2)_, read "big oh of _n_ squared" or just "oh of _n_ squared," we mean that there are positive constants _c_ and _n0_ such that for _n_ equal to or greater than _n0_, we have _T(n) <= cn^2_.»

Alfred Aho, Data Structures and Algorithms

### Big-Oh notation

«To talk about growth rates of functions we use what is known as "big-oh" notation. [..] When we say the running time _T(n)_ of some program is _O(n^2)_, read "big oh of _n_ squared" or just "oh of _n_ squared," we mean that there are positive constants _c_ and _n0_ such that for _n_ equal to or greater than _n0_, we have _T(n) <= cn^2_.»

Alfred Aho, Data Structures and Algorithms

### Big Omega notation: lower bound of the growth rate

«To specify a lower bound on the growth rate of _T(n)_ we can use the notation _T(n)_ is _Ω(g(n))_, read "big omega of _g(n)_" or just "omega of _g(n)_," to mean that there exists a positive constant _c_ such that _T(n) ≥ cg(n)_ infinitely often (for an infinite number of values of _n_).»

Alfred Aho, Data Structures and Algorithms

## Measuring Running Times

### Average Running Time

«We also consider _Tavg(n)_, the average, over all inputs of size _n_, of the running time on that input.»

Alfred Aho, Data Structures and Algorithms

### Worst case running time

«we define _T(n) to be the _worst case_ running time, that is, the maximum, over all inputs of size _n_, of the running time on that input.»

Alfred Aho, Data Structures and Algorithms

### Worst Case Scenario as the default measurement

«In practice, the average running time is often much harder to determine than the worst-case running time, both because the analysis becomes mathematically intractable and because the notion of "average" input frequently has no obvious meaning. Thus, we shall use worst-case running time as the principal measure of time complexity, although we shall mention average-case complexity wherever we can do so meaningfully.»

Alfred Aho, Data Structures and Algorithms

### Computer speed and the largest problem we can solve

«unless a program has a low growth rate such as _O(n)_ or _O(nlogn)_, a modest increase in computer speed makes very little difference in the size of the largest problem we can solve in a fixed amount of time.»

Alfred Aho, Data Structures and Algorithms

### The impact of speed improvement on running time

«We observer that a 1000% improvement in computer speed yields only a 30% increase in the size of problem we can solve if we use _O(2^n)_ program.»

Alfred Aho, Data Structures and Algorithms
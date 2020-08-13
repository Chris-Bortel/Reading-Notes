# Read-09

[README](/README.md)

## [Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

Functional programming is a programming paradigm
- A style of building the structure and elements of computer programs
- Treats computation as the evaluation of mathematical functions
- Avoids changing-state and mutable data — Wikipedia


Pure functions
- Is deterministic: returns the same result given the same args
- Has no observable side effects

Stuff that is not pure
- Reading files : If a function reads external files, it’s not a pure function — the file’s contents can change.
- Random number generation : Any function that relies on a random number generator cannot be pure.


Immutability
- Means that data is unchanging over time or unable to be changed
- NOTE: State cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.


## [Refactoring Javascript for Readability](https://dev.to/healeycodes/refactoring-javascript-for-performance-and-readability-with-examples-1hec)

When refactoring, it is important to keep a middle ground. Code should not be so fast that we cannot understand it. 


### BeWare
Be careful if you're iterating through a flat array very often, especially if it's a core piece of your program. The refactor will change the data-structure of URLstore.



A function should do one thing. Break up your functions so that they can keep being used when the company grows. 


No duplicate code. ONE code to Rule them All!
- write one function that accepts a list of friendly things.



### Strategies for writing clean code
- Return early from functions
- Cache variables so functions can be read like sentences
- Check for web APIs before implementing you own functionality
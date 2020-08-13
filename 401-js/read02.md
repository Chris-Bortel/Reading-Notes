# Read: 02 - Classes, Inheritance, and Functional Programming

[README](/README.md)

## Research
- Name 3 advantages to Test Driven Development
  - Allows us to check code as we go so that we know that we are working with polished code. It speeds up development. Development starts expensive, and then it gets cheaper as we move forward. 
    - Reproducible build
    - gives us reusible robust test suite and allows us to refactor
    - leads to evolutionary code
    - KISS Principle - focus on development of code 


- In what case would you need to use beforeEach() or afterEach() in a test suite?
  - Setup and Teardown
  - you have some finishing work that needs to happen after tests run. beforeEach() and afterEach() are helper functions provided by jest


- What is one downside of Test Driven Development
  - lot of time and effort up front, making development feel slow in the beginning
  - focusing on the simplest design now and not thinking ahead can lead to major refactoring requirements
  - difficult to write good tests
  - Tests need to be maintained when requirements change


- What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?
  - a class defines a type which can be instantiated at runtime, 
  - a prototype is itself an object instance


- Name a use case for a static method
  - Use static when you want to provide class level access to a method, i.e. where the method should be callable without an instance of the class. Static methods don't need to be invoked on the object and that is when you use it. Example: your Main() is a static and you don't create an object to call it.


- Write an example of a Higher Order function and describe the use case it solves
  - map function on arrays.
  - Higher-order functions allows you to write simpler and more elegant code.
  - use case: have an array with multiple objects. Gives an array containing only a piece of the object that you need.



## Terms to understand
[Master the JavaScript Interview: What is Functional Programming?](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0)
- functional programming
  - the process of building software by composing pure functions, avoiding shared state, mutable data, and side-effects.
  - is declarative and application state flows through pure functions
  - more concise, predictable, and easier to test


- pure function
  - Given the same inputs, always returns the same output, and
  - Has no side-effects


- higher-order function
  - function which takes a function as an argument, returns a function, or both. Higher order functions are often used to:
    - Abstract or isolate actions, effects, or async flow control using callback functions, promises, monads, etc…
    - Create utilities which can act on a wide variety of data types
    - Partially apply a function to its arguments or create a curried function for the purpose of reuse or function composition
    - Take a list of functions and return some composition of those input functions

- immutable state
  - an object that can’t be modified after it’s created (not const: const creates a var name that can;t be reassigned after creation. can;t change the obj that in being bound, but you can still change the proberties of the object)
  - this is a central concept of functional programming, without it, the data flow in the program is lossy

- object
- object-oriented programming (OOP)
- class
- prototype
- ``super``
- inheritance
- constructor
- instance
- context
- this
- Test Driven Development (TDD)
[Medium Article On TDD](https://medium.com/@stevenpcurtis.sc/test-driven-development-tdd-the-advantages-and-disadvantages-5347899ead90)
  - A technique that allows you to make sure that code does what you thing it does. It is useful for JS because cross-brower incompatibilities mess you up.
  - With TDD, intentions are expressed twice: once as a test, and onvr sd ptofuvyion code. If these to instances do not match, there must be a bug.
- Jest
- Continuous Integration (CI)
- unit test


# Take Away about functional programming Pros
- Pure functions instead of shared state & side effects
- Immutability over mutable data
- Function composition over imperative flow control
- Lots of generic, reusable utilities that use higher order functions to act on many data types instead of methods that only operate on their colocated data
- Declarative rather than imperative code (what to do, rather than how to do it)
- Expressions over statements
- Containers & higher order functions over ad-hoc poly

# Read: 11 - Authentication


[README](/README.md)

Explain what a “Singleton” is (in Computer Science terms) [what is a singleton?](https://medium.com/better-programming/the-complete-guide-to-the-singleton-design-pattern-dd0e7a5a4dc)
- **It makes sure that a instantiation  of a class only has one instance**
- a class that has it's own attribute called unqueInstance that stores an instance of the Singleton class. The class constructore is privatte and can only be access through and accessor method. the accessor method is responsible for returning the single instance or if it does not exist, then it will create a new instance
  - making multiple instances of one object could be prblematic
  - in the above article, he is making logger into a singleton which reuses one instance of the class
 - could be thought of as an alternative to global variable or static classes.
- unlike global variable, singletons to dot take oup spance in the namespace
- Q: are they easier to initialize? What does that mean?

Explain how the Singleton pattern can be used with Node modules, specifically with classes [Node.js Design Patterns — Singleton pattern ( Series -1)](https://medium.com/@maheshkumawat_83392/node-js-design-patterns-singleton-pattern-series-1-1e0ab71e3edf)

- we use a singleton pattern when we want ot make sure that you have one and only one instance of an object
- They now have 3 instances of logger, one in each file, but we are only able to look and the first instance that was created within our main app/ 
  - we do not want multiple instances of the logger class

If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?
Document the following Vocabulary Terms
- 

Term
Router Middleware
Dynamic Module Loading
Singleton Pattern
CRUD -> REST Method Matches
Mock Testing
# Read 27: 11-4-2020

## Props and State

[README](/README.md)

### Questions

1. Does a deployed React application require a server?
    - sort of. react has it all built in and ready to go
1. Why do we prefer to test a React application at the behavior rather than the unit level?
    - Because the behavior is what we are interested in as it is the output that the user will be seeing
1. What does npm run build do?
    - Creates a production build of your application in the /build folder

<!-- 1. Describe the actual composition / architecture of a React application -->

### Vocabulary Terms

1. [BDD](https://www.scaledagileframework.com/behavior-driven-development/)
    - Behavior Driven Development : "A Test-First, Agile Testing practice that provides Built-In Quality by defining (and potentially automating) tests before, or as part of, specifying system behavior."
    - It can be brittle, and not test all cases.

1. Acceptance Tests
    - Checks whether or not your application is behaving the way that the user expects it to.

1. Mounting --- [React Docs](https://reactjs.org/docs/react-component.html)
    - Methods that are called when when a component is being created and inserted in the DOM
    - constructor() , render() , componentDidMount()

1. Build --- [React Docs - optimizing performance](https://reactjs.org/docs/optimizing-performance.html)
    - It optimizes your applications performance.

# Read 31: 11-14-2020

## Routing

[README](/README.md)

### Questions

1. Do child components have direct access to props/state from the parent?
 - Child components need the parent component to send the props to them

2. When a component “wraps” another component, how does the child component’s output get rendered?
  - It needs to have a function from the wrapper to send the data to the component to be rendered

3. Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?
  - Yes?

4. What trick can a parent use to share all props with it’s children.
- Just set the initial state to use the parents state.

### Vocabulary Terms

1. props.children - It passes children elements directly into their output.

2. composition - composition is how the JSX sends data around. Passing stuff top down

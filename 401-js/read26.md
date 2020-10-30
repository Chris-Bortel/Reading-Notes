# Read 26: 10-30-2020

## Component Based UI

[README](/README.md)

### Questions

1. Name 5 [Javascript UI Frameworks](https://hackr.io/blog/best-javascript-frameworks) (other than React)
  - [Angular](https://hackr.io/blog/best-javascript-frameworks)
  - [Ember.js](https://guides.emberjs.com/release/)
  - [Vue.js](https://vuejs.org/)
  - [Mithril](https://mithril.js.org/)
  - [Aurelia](https://aurelia.io/)

2. What’s the difference between a framework and a library?

[freeCodeCamp](https://www.freecodecamp.org/news/the-difference-between-a-framework-and-a-library-bd133054023f/) explains this so well.

- Library : "Is like going to Ikea. You already have a home, but you need a bit of help with furniture. You don’t feel like making your own table from scratch. Ikea allows you to pick and choose different things to go in your home. You are in control."

- Framework : "Is like building a model home. You have a set of blueprints and a few limited choices when it comes to architecture and design. Ultimately, the contractor and blueprint are in control. And they will let you know when and where you can provide your input."


JSX Prevents injection attacks and is there for safe to embed user input while using JSX

React.createElement() performs checks automatically and helps you write bug-free code while producing a fairly basic object. 

``` 
// Input
const element = React.createElement(
  'h1',
  {className: 'greeting'},
  'Hello, world!'
);

// Output
// Note: this structure is simplified

const element = {
  type: 'h1',
  props: {
    className: 'greeting',
    children: 'Hello, world!'
  }
};
```

### Vocabulary Terms

1. Rendering : Rendering sends elements and components to the dom. Once react elements are rendered, they are immutable, you cannot change its children or attributes. Brings DOM to the desired state

2. Templates : Are prebuilt components to use instead of building them from scratch.

3. State: "React components have a built-in state object. The state object is where you store property values that belongs to the component. When the state object changes, the component re-renders." - [W3Schools](https://www.w3schools.com/react/react_state.asp)

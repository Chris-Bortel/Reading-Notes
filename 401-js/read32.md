https://docs.google.com/document/d/1NJVK0YrTH66vSXw7Y7qRIsRrkE7uapz0wfG4h3IzI7c/edit?usp=sharing# Read 28: 11-7-2020

[Link to Directory](/README.md)
## Custom Hooks
## [Assignment Link](https://canvas.instructure.com/courses/2168372/discussion_topics/9374379/submit)

## **Questions**
1. What does a component’s lifecycle refer to?
    - Three main phases. The three phases are: Mounting, Updating, and Unmounting.
1. Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect
    - Allows us to prevent the re-creation of a function. Functions are objects, we do not want to create more objects than we want
    - With out useCallback(), any function that is defined within the useEffect() will be recreated whenever the component rebuilds
    - [Resource from Medium](https://medium.com/@infinitypaul/reactjs-useeffect-usecallback-simplified-91e69fb0e7a3)
1. Why are functional components preferred over class components?
    - They are easier to work with
    - Benefits:
      - Functional component are much easier to read and test because they are plain JavaScript functions without state or lifecycle-hooks
      - It has less code which makes it more readable
      - It will get easier to separate container and presentational components because you need to think more about your component’s state if you don’t have access to setState() in your component
      - [Resource from Medium](https://medium.com/wesionary-team/react-functional-components-vs-class-components-86a2d2821a22)

1. What is wrong with the following code?





## **Terms**
1. State hook
    - useState() allows us to add React state to a function components
1. Effect hook
    - useEffect() allows us to perform side effects in function components
    - **So, what does it do?** 
      - "By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API."
      - [React Docs, **Important!**](https://reactjs.org/docs/hooks-effect.html)


1. Reducer hook
    - "An alternative to useState. Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method." (It is like redux.)
      - [React Docs](https://reactjs.org/docs/hooks-reference.html#usereducer)



    

<br>
<br>
<br>
<br>

## Preparation Materials
### Authoring

- [custom hooks - all you need to know](https://www.telerik.com/kendo-react-ui/react-hooks-guide/#toc-custom-react-hooks)
- [async hooks](https://dev.to/vinodchauhan7/react-hooks-with-async-await-1n9g)
- [useReducer Hook](https://reactjs.org/docs/hooks-reference.html#usereducer)
- [react custom hooks](https://reactjs.org/docs/hooks-custom.html)

### Hooks Lists/Collections

- [use hooks](https://usehooks.com/)
- [hooks list](https://github.com/rehooks/awesome-react-hooks)
- [10 essential react hooks](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d)





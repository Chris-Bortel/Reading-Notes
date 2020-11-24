# Read 33: 11-24-2020

## Context API

[README](/README.md)

### Questions

1. Describe use cases for useMemo() and [useReducer()](https://reactjs.org/docs/hooks-reference.html#usereducer)

- `useMemo()` returns a [memoized](https://en.wikipedia.org/wiki/Memoization) value.
  - 'UseMemo will only recompute the memoized value when one of the dependencies has changed. This optimization helps to avoid expensive calculations on every render.'
  - Functions passed to `useMemo` run during rendering.
  - **Sounds as though the is a `useEffect()` that is optimized**

- `useReducer()` is an alternative to useState(), it takes a reducer of type ``(state, action) => newState`` and returns the current state paired with a dispatch method
  - you should use this instead of useState when there is complex state logic that involves multiple sub values or when the next state depend on the previous one
  - 'It is **Important** to note that `useReducer` also allows us to optimize performance for components because we can trigger deep updates because you can pass [dispatch](https://reactjs.org/docs/hooks-faq.html#how-to-avoid-passing-callbacks-down) down instead of callbacks using **context**. this is the recommended pattern for deep ??updates?? '  ??WHAT IS A DEEP UPDATE??

2. Why do custom hooks need the use prefix?
- Just a naming convention

3. What do custom hooks usually do?
- hooks extract data to be reused. They make code more efficient and easier to read.d
4. Using any list of custom hooks, research and name one that you think will be useful in your applications.
- The form hook was helpful in my application

5. Describe how a hook that fetches API data might work
- It has all of the logic that any other call would have, but it uses use effect and it called by render with less code up front.

### Preparation Materials
- [context api](https://reactjs.org/docs/context.html)
- [hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)
- [react context links](https://github.com/diegohaz/awesome-react-context)
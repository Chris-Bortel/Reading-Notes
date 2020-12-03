# Read 33: 12-2-2020

## `<login />` and `<Auth />`
maybe this will work , what do you think senior wrist and top of hands?
so I will probably try
[README](/README.md)

### Questions

1. Why is the Context API useful?
- “Context provides a way to pass data through the component tree without having to pass props down manually at every level.”
- It allows all components to have the opportunity to be given access to state in the context level

2. Can a component outside of a provider get its context?
- No, is a top down system

3. What are some common use cases for using the Context API?
- When you have state that needs to be passed around the component tree. It is way cleaner than sending props all over the place from the parent.

4. Describe “Context Hell”
- A big mess of nested context that gets difficult to scope properly

### Vocab

1. global state
- It is state that can be accessed by the entire application

2. [global context](https://reactjs.org/docs/context.html)
- "Context provides a way to pass data through the component tree without having to pass props down manually at every level."

3. provider
- The context parent that feeds all of it's children

4. consumer
- The kid that takes the state a good stuff from the context if it wants it

### Helpful Resources

* [What is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)
* [React-cookies component](https://www.npmjs.com/package/react-cookies)
* [React-cookie library](https://www.npmjs.com/package/react-cookie)
* [Provider Pattern with react context API](https://blog.flexiple.com/provider-pattern-with-react-context-api/)
* [Working with react context API](https://www.toptal.com/react/react-context-api)
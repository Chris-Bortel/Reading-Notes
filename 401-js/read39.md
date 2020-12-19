# Read 37: 12-11-2020
## Redux - Additional Topics
## [Assignment Link](https://canvas.instructure.com/courses/2168372/discussion_topics/9374372)

## **Questions**
1. What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application? 
- We want to use combineReducers which will bundle all of the initial state and render it

1. When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
- We dispatch the the axios call but more specifically, we are sending the payload with the api response. 

## **Terms**
1. middleware
- Is any software that is hit on the way from your server to the client. We do stuff with it in order to modify our data 
- "In this case, Redux middleware function provides a medium to interact with dispatched action before they reach the reducer. Customized middleware functions can be created by writing high order functions (a function that returns another function), which wraps around some logic. Multiple middlewares can be combined together to add new functionality, and each middleware requires no knowledge of what came before and after. You can imagine middlewares somewhere between action dispatched and reducer." [Redux Middleware](https://www.tutorialspoint.com/redux/redux_middleware.htm#:~:text=In%20this%20case%2C%20Redux%20middleware,which%20wraps%20around%20some%20logic.)

1.[thunk]https://daveceddia.com/what-is-a-thunk/
- A middleware
- It calls actions that are functions (and returns whatever they return), and otherwise passes the action along to then next middleware, or to Redux itself (which is what next(action) does).
- It returns the action obj in a nice little package.


## **Preparation Materials**
- [Redux Toolkit(RTK)](https://redux-toolkit.js.org/)
- [Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)
### Alternative State Managers
- [MobX](https://mobx.js.org/getting-started.html)

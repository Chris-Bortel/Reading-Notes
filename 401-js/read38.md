# Read 41: 12-15-2020
[Link to Directory](/README.md)
## Redux - Asynchronous Actions
## [Assignment Link](https://canvas.instructure.com/courses/2168372/discussion_topics/9374373)

## **Questions**
1. How granular should your reducers be? [Redux Style Guide](https://redux.js.org/style-guide/style-guide)
    - Reducers should be very specific to cut down on render time of components. If a component does not need a particular piece of data, there is no reason to give it to them.

1. Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
    - Pro, as long as you are cognizant of what is being fired and what data you want to be sent 
1. Name a strategy for preventing the above. 
    - Using a namespace will allow you to keep reducers separate when being called. 

## **Terms**
1. store --- [Redux](https://redux.js.org/understanding/thinking-in-redux/glossary#store)
    - An object that hold the application's state tree. Has methods to send the state around: 
    - dispatch(action) is the base dispatch function described above.
    - getState() returns the current state of the store.
    - subscribe(listener) registers a function to be called on state changes.
    - replaceReducer(nextReducer) can be used to implement hot reloading and code splitting. Most likely you won't use it.
1. combined reducers --- [Redux](https://redux.js.org/api/combinereducers)
    - A helper function that combines multiple reducing functions into a single one that you can pass to createStore
    - The combined reducer calls every child reducer, and gathers their results into a single state object. 
    - "The state produced by combineReducers() namespaces the states of each reducer under their keys as passed to combineReducers()"

<br>
<br>
<br>
<br>

## **Preparation Materials**

- [Async actions](https://redux.js.org/tutorials/fundamentals/part-6-async-logic)
- [Thunk middleware](https://github.com/reduxjs/redux-thunk)
- [Redux thunk](https://www.digitalocean.com/community/tutorials/redux-redux-thunk)

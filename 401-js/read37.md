# Read 37: 12-11-2020
## Redux - Combined Reducers
## [Assignment Link](https://canvas.instructure.com/courses/2168372/discussion_topics/9374375)

## **Questions**
1. Why choose Redux instead of the Context API for global state?
    - Once wired, Redux allows us to manage state of a large application much easier than the context Api
1. What is the purpose of a reducer?
    - They allow your react application to have specific pieces of data that all update synchronously.  All reducers run against your Redux store, and then the store triggers a change event and your entire React.js application re-renders.
1. What does an action contain?
    - Type and Payload 
1. Why do we need to copy the state in a reducer?
    - Because of states immutable nature, we need to copy the state before we modify it in any way

## **Terms**
1. Immutable state
    - Cannot be modified
1. Time travel in redux
    - Time travel is the ability to move back and forth among the previous states of an application and view the results in real time.
    - We use Redux DevTools Extension to do this. [Resource](https://blog.scottlogic.com/2017/03/09/relogic-2.html)
1. Action creator
    - A function that returns an action object. [Redux Book](https://read.reduxbook.com/markdown/part1/04-action-creators.html)
1. Reducer
    - Allows you to send modify the state.    
1. Dispatch
    - Sends out the reducers so that components may use them.


## **Preparation Materials**
- [Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)
- [Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)
- [Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

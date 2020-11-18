# Read 31: 11-17-2020

## Hooks API

[README](/README.md)

### Questions

1. Why do we not need more .html pages in a multi-page React app?
  
  - We do not need more .html pages, because all of the structure of the application in housed in the components themselves, and then rendered in App in the order that we want them to appear. 

2. If we wanted a component to show up on every page, where would we put it and why?

  - Outside the <BrowserRouter/>
    - because on render it will appear 
  - Inside the <BrowserRouter />, outside a <Route />
  - Inside a <Route /> 


### Term

- Composition : is used in order to reuse code between components. It is how we pass children elements directly into their output. This uses props.children

- Children / Child Components -- [A deep dive into children in React](https://mxstbr.blog/2017/02/react-children-deepdive/#child-components)
  - there is a parent component, such as <Grid/>, and that grid can have multiple child components such as three <Row/> components. They are passed using props.children 

  - parents do not have to render their children, though I do not know why not. Why do they even have children then 
  - You can manipulate children using React.Children

- Hash Routing -- [HashRouter](https://reactrouter.com/web/api/HashRouter)
  - "A <Router> that uses the hash portion of the URL (i.e. window.location.hash) to keep your UI in sync with the URL."

- Link Routing : allows you to navigate through your application using links.


## Hooks and the like

  [making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

  - Cool thing about hooks --- There seems to be a `useState()` function that will use all of the local state without the binding stuff

  ![]('../401-js/img/read31-making-sense-of-hooks.png')

  - you do not need to set the state or this.state.whatever. You  just use useState() with a variable name. **these** are HOOKS!!

  - hooks can be used more than once in a component...
  ![]('../401-js/img/read31-making-sense-of-hooks2.png')
  
  
  ![]('401-js/img/read31-making-sense-of-hooks3.png')

  - theme context??? LocalContext

### How does react know which useState call cooresponds with which state call

- react relies on the order of these calls
- **IMPORTANT** the rule is that you can not call hooks inside of a condition, it has to be at the top level of your component

### side effects and hooks
  ![]('../401-js/img/read31-making-sense-of-hooks3.png')

- we can import useEffect.> use effect runs prior to render and as you update

- useEffect hooks are consistent and is declared inside of the component instead of outside 

### useEffect

- use  effects to handle multiple side effects

- Effect hooks have a cleanup phase. any effect can return a function, which is where we unsubscribe and end the effect. This means addEventListener and removeEventListener

with hooks we separate code based on what the code is doing

## Important, hooks are just function calls
- components are just functions
- you share logic between two functions by extracting it to a new function. 

### Custom hooks 00:47:00 in the above video

### Questions. 

- you can have multiple state variable?

## hooks allow us to...

 - use all react feature without a class
 - reuse stateful logic between components without wrapper hell



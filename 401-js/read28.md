# Read 28: 11-7-2020

[Link to Directory](/README.md)
## Component Composition
## [Assignment Link](https://canvas.instructure.com/courses/2168372/discussion_topics/9374383)

## **Questions**
1. Can a parent component access the state of a child component?
   - You can do this by using a callback function

1. What can be passed along in a prop variable?
    - A prop is just an object. We can pass anything in it. 

1. How can a child component “know” the state of another component?
    - It can only receive the state by props being passed to the parent and then to the component that is wanting it.


## **Terms**
1. Component props
    - Allows us to send reusable pieces of ui
    - props get passed to the component (similar to function parameters)
1. Component state --- [React Docs](https://reactjs.org/docs/faq-state.html#gatsby-focus-wrapper)
    - is managed within the component (similar to variables declared within a function).
1. Application state
    - It is the memory of the application. It is the point in time that the application currently is depending on how it has been interacted with.
    - NOTE: I like this definition found on [Stack Overflow](https://stackoverflow.com/questions/8102674/what-is-application-state#:~:text=An%20application%20state%20is%20simply,previous%20version%20of%20the%20page.)
      - An application state is simply the state at which an application resides with regards to where in a program is being executed and the memory that is stored for the application. The web is "stateless," meaning everytime you reload a page, no information remains from the previous version of the page. All information must be resent from the server in order to display the page.
      - Technically, browsers get around the statelessness of the web by utilizing techniques like caching and cookies.

    

<br>
<br>
<br>
<br>

## **Preparation Materials**

[react basics recap](https://www.freecodecamp.org/news/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030/)
<br>

[props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)
<br>

[composition vs inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)
<br>

[react testing library api example](https://testing-library.com/docs/react-testing-library/example-intro)
<br>

[react-if-component](https://www.npmjs.com/package/react-if)
<br>

[react-testing-library-async](https://testing-library.com/docs/dom-testing-library/api-async)


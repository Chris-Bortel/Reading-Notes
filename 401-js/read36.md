# Read 36: 12-8-2020

## [Assignment](https://canvas.instructure.com/courses/2168372/discussion_topics/9374375)

## **Questions**
**What are the advantages of storing tokens in “Cookies” vs “Local Storage”?** [Medium Article](https://medium.com/datadriveninvestor/cookies-vs-local-storage-2f3732c7d977#:~:text=Cookies%20and%20local%20storage%20serve,you%20more%20to%20work%20with.)
- Cookies are mainly for reading server-side, whereas local storage can only be read by the client-side.
- Local storage is a very permanent solution, where cookies are time sensitive 
- cookies hold plenty of info, and are located on a user's computer, data specific to a client and website, and they can accessed either by the web server or the client computer.
- With cookies we do not need to use up a bunch af data in a server machine. 
- Without using cookies, it is difficult to retrieve user info with out requiring a login on each visit.
- "A cookie can simply be used if there is a large amount of information to store. In addition a cookie can be made to persist for an arbitrary length of time."


**Explain 3rd party cookies.** [ClearCode](https://clearcode.cc/blog/difference-between-first-party-third-party-cookies/#:~:text=Third%2Dparty%20cookies%20are%20those,services%2C%20such%20as%20live%20chats.) 
- "Created by domains other than the one the user is visiting at the time, and are mainly used for tracking and online-advertising purposes. They also allow website owners to provide certain services, such as live chats." They can also increase the risk of invasion of privacy and security risk to the websites utilizing them.


**How do pixel tags work?** [Quora](https://www.quora.com/How-does-a-tracking-pixel-work)  
- They are used by advertisers to collect user data for web, mobile, and email marketing. HOW THEY WORK --- "A pixel code snippet is added to the HTML code of a website or email, the pixel will begin to track various information about the visitor viewing the document. This user data is collected when the tracking pixel is loaded via the visitor's browser. Once the tracking pixel is processed in the browser it is known as the pixel "firing", which means the visitor's data was sent to the pixel server collecting the information."


## **Term**

**Cookies** - Small files which are located on a user’s computer. They hold a generous amount of data specific to a client and a website, they can be accessed by either the web server or the client server. Cookies allow the page to be rendered for the specific user, it saves some of the information in a safe manner. They are key value pairs, and the value is data.

**Authorization** - Allows users to access there information and gives them the ability to do tasks base on their roles... i.e not every user is authorize to make the same actions.

**Access control** [Medium Article](wXE85g9fMEGJKur85XrOOfUCOANm14ALREAWcX6A37WqzIZwqlY4uSYKfwDBjcr1zExLeLB88a7MmOJQ35f2pQXM4vKbe5m1VSG91i2C3LSqAIRJguaklvktX222uaw) - It makes sure that employees or users are only able to access the resources that they are authorized to view. It restricts them from letting users see info that is irrelevant to their job duties (i.e. financial data, customer info, etc.)

**Conditional rendering** - `If` `Else` statements. "It refers to the process of delivering elements and components based on certain conditions being met."


## **Helpful Links and Notes That Are Not Really Organized (Redux):**

#### [Dan Abramov Redux Tutorials](https://egghead.io/courses/getting-started-with-redux)
### Notes:
Entire state of you application will be in one js obj
mutations and changes are explicit
- **state tree is read only ---- any time that you want to make a change to the state, you need to dispatch an action ---- the action is the minimal representation of the change to that data.**
- !! There are different types or actions that are used in different types of apps.
  - In a counter app we only have increment and decrement actions (no additional info is passed because we are only focussed on the counter changer)have an add action
  - We could also have a remove counter action , that shows the index when we add or decrement. We need to see what component has an action done to it
  - When we add a todo 

  **any data that gets into a redux application gets there by actions**

  - Need to understand the importance of pure and impure function 
  - Pure functions just calculate hte the new value. They are functions whose returned value depends solely on the values of their arguments

#### [Worlds easiest guide to redux](https://www.freecodecamp.org/news/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6/)
 - The state of the application is kept safe by something called a store... It is like the bank vault of the application

### Redux principles
1. Single source of truth (one state to rule them all)
2. State is read only, the only way to change the state is to **emit** an **action** ---> an action is an object TAKES a type field that describes what you want your action to do, and then what you want to do
3. To specify how the state tree is transformed by actions, you write pure reducers

#### [testing redux](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)
#### [Redux Docs](https://redux.js.org/)




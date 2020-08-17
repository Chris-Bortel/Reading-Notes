# Read: 01 - Node Ecosystem, TDD, CI/CD 


[README](/README.md)

## Reading, Research, and Discussion

Why would you want to run JavaScript code outside of a browser?
- I answered this below

What is the difference between a module and a package? 
- I answered this question down below and used [stack overflow](https://stackoverflow.com/questions/20008442/difference-between-a-module-and-a-package-in-node-js#:~:text=A%20module%20is%20a%20single,has%20metadata%20about%20the%20package.&text=Now%20it's%20very%20common%20for,a%20package%20as%20a%20module.
) as a resource.


What does the node package manager do?
- allows users to access open sourced project to use in their own code. This speeds up development and allows for better code. 

Provide code snippets showing 3 different ways to export a function from a node module
```
module.export('')
```

```
module.exports = function (firstName, lastName) {
    this.firstName = firstName;
    this.lastName = lastName;
    this.fullName = function () { 
        return this.firstName + ' ' + this.lastName;
    }
}
```




## Vocabulary terms

ecosystem
- is a collection of software packages, libraries, and other resources that facilitate development as they integrate with each other.
- [Medium overview of the js ecosystem](https://medium.com/@krposlek/overview-of-the-javascript-ecosystem-8ec4a0b7a7be)
Node.js
- allows us to run js without/outside of a browser. 
- we want to do this because it lets us communicate with the database and do stuff...

V8 Engine
- V8 provides the runtime environment in which JavaScript executes. The DOM, and the other Web Platform APIs are provided by the browser. -- [node.js](https://nodejs.dev/learn/the-v8-javascript-engine)
- is used in the chrome engine as well as node.js. It makes looping over arrays super effient... It makes stuff fast

module
- modules are libraries for node.js
- a single js file that has some reusible code

package
- is one or more modules (AKA libraries)
- directories that have one or more files in it. Includes a package.json  ... has reusible-code.
- these packages are often small chunks of code to be building blocks to solve stuff;

node package manager (npm)
-  is an online repository for puplishing open-source node.js projects.
- is also a command-line for interacting with those repositories and installing those packages

server
- serves thing to the client. It is the middle man between the client and the database/api. It does the retrieving and delivering
environment
interpreter
compiler

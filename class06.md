# Read 06
[GitHub Repo](https://github.com/Chris-Bortel/Reading-Notes)

# Chapter 3: “Object Literals” (pp.100-105)
 - you create an object literal by:
  - The object is the curly braces and their contents. The object is stored in a variable called hotel. Therefore, you refer to it as the hotel object. 
  - you can access an object with dot notation
 -below is an object built with literal notation --- is literal notation just dot notation?
  ```
var hotel = {
name: 'Quay',
rooms: 40,
booked: 25,
checkAvailability: function() {
return this.rooms - this.booked; }
JAVASCRIPT
8 FUNCTIONS, METHODS & OBJECTS
};
  ```
# Chapter 5: “Document Object Model” (pp.183-242)

Dom: Docoument Object Model specifies how browsers should create a model of an html page and how js can access and update the contents of a page while in the browser window.
- not part of html or js
The DOM specifies the way thata the browser should structure this model using a dom tree
-You will hear people call the DOM an 1 Application Programming Interface (API).

### Model of a loaded page
You are seeing the DOM tree
**EXAMPLE** pp 186
- HTML is represented by its own DOM node.
At the top of the tree a document node is added; it represents the entire page

### Don't cha **Node**
Each node is an object with methods and properties.
- Scripts access and update this DOM tree **(not the source HTML file).** Any changes made to the DOM tree are reflected in the browser.

### Working with da DOM Tree
- STEP 1: Access the elements
- Step 2: work with those elements

--- When people say that the Dom is working with an element, it is actually working iwiht a node that represents that element.






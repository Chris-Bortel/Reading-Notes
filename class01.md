Read: 01 - Introductory HTML and JavaScript
3/29/20

# HTML Chapter 1: “Structure” (pp.12-39)
### Summary/Things to look out for while reading 

***************
* HTML pages are text documents.
* HTML uses tage (characters that sit inside angled brackets)to give the info they surround special meaning 
    - Tags are often referred to as elements 
    - Usually come in pairs < >
    - Opening tags carry attributes, which tell us more about the content of that element
    - Attributes require a name and a value
    - Learn where tags can go and what they are used for 
**************
This is what HTML structure looks like. 
``` 
<html>
    <body>
        <h1> Heading </h1>
        <p> Paragraph  </p>
        <h2> Subheading </h2>
        <p> Supporting paragraph </p>
        <h2> Another subhead </h2>
        <p> Paragraph <p>
    </body>
</html>

```
Make sure to use both opening and closing tags.
 - Tags act as container that tell you about the content

 ***********

### Attributes
```
<html lang="en-US">
```
- Attr tells us information about the content that is inside of the tags. The above snippet denotes that the html content is in english. 
*************

### Content Management System
- Allows clients to modify one template in order to modify content throughout the website. This is easier than having to modify every single item throughout the site.

## Conclusion
HTML Structure is the base of a website, and controls what content is visible and how it is presented. 

************
************
************

# HTML Chapter 8: “Extra Markup” (p.176-199)
//
## DOCTYPES
DOCTYPE is a declaration that tells the browser which HTML version is being used.
- Current HTML doctype that is use is HTML5
    - Other versions include HTML4, Transitional XHTML 1.0, Strict XHTML 1.0, and XML Declartion 

### Comments In HTML
"<!- ->" Uses double dashes, but allows us to put in notes that tell us what we are doing in the code. This can also be used to "comment out" Code so that it is not rendered in the browse.

### ID Attributes
```
<h1 id="heads"> .... </h1>
```
Known as a global attribute because it can be used on any element.
This allows us to target this element in CSS and manipulate how it is formatted. I CSS it is denoted with.

```
#heads {
    background: blue;
    font-style: calbria;
    etc...
}
```

### Class Attribute
This is similar to the ID attribute, but it can be used to target specific elements in the page.
```
<p class class="important> ... </p>
```
```
.important  {
    font-weight: bold;
}
```

### Block Elements
These elements always appear to start on a new line in the browser 
- includes:
```
<h1>, <p>, <ul>, <li>
```
### Inline Elements
Always appear as though they continue on the same line as their neighbors.
- includes:
```
<a>, <b>, <em>, and <img>
```
### Grouping Text and Elements In A Block
We do this by using the Div tag
```
<div id="content>
    <h1> ... </h1>
    <p> ... </p>
    <p> ... </p>
</div>
```

### Span
Another way to target specific elements in your code. This is used inline opposed to targeting the entire block of code. 
This will put your code in a seperate box that allows you to move it around, modify content within it as well as many other things
    
```
<p> A bow tie is a <span style="text-wieght: bold"> bold </span> choice </p>

```
## More Markups!

### iframe
A page withing a page. Can be used to put a map in or some other object.
```
<iframe>
```

### Meta Tags
These are cool because you can put description of what the page is all about with out having it rendered to the browser
```
<meta name="description"
    content="telling us what the description of something is>

```

//
************
************
************










# HTML Chapter 17: “HTML5 Layout” (pp.428-451)
HTML5 give us elements that allow us to use less DIV elements to format the our documents. The provides us with cleaner code!
- They also are describe what different sections of codes do more clearly than listing div with classes.
_ These tags include: content, aside, nav, article
- These provide more readable code making it easier to come back later and work with

//
//
************
************
************
# HTML Chapter 18: “Process & Design” (pp.452-475)

### Understand target audience
#### Who is the site for!?
- It is important to figure out who the site is for, who will be utilizing it, and what the goal is that the site is fullfilling. 
#### Why are people coming to the site?
//
We can answer this by listing/ discovering why the key motivators why someone would use the site.
- Examine the goals of the visitor
    - Shopping
    - Gaining information
    - Recreation
    - Looking for services
    - Wanting to reach out to the company or individual that the site is built for
- Figure out what information viewer are looking for on the website. This will allow you to make the site useful and most importantly, utilized. 

### Psuedo Code
### Site mapping - form a plan for the stucture of a site. 
//
A diagram that shows the pages that will be on the site and the order/structure that they will be presented/grouped in. 
- This shows the hierachy of the site. 
- Could include:
    - Home page
        - About and what will be inside of that section.
        - Articles ...
        - Contacts - How to get ahold of the company
        - etc...
#### Wireframes are your friend
//
The main purpose of this tool is to show the devopers and clients a vague layout of what the website and its pages will looklike and how they will flow together
- Organizes thoughts for what needs to happen on each page and how to execute it.


### Make sites obvious.
//
People should know what your site is trying to accomplish.
- Visual hierachy is a helpful tool to get this done.
- A well thought out and easily uderstandable navigation method is an important tool in order to make a site usefull and approachable.
    Nav bar should be/have
    - Concise
    - Clear
    - Selective - only displaying the different sections or content of the site.
    - Context - Should make sense why the different section are there and how they relate to each other.
    - Should be easy to interact with. 
    - All nav features should work that same throughout the site.
        - Users do not want to have to guess how to get around.
**IMPORTANT**
When writing scripts, the goal **MUST** be broken down into a series of small/digestible tasks


*************
*************
*************

# JS Chapter 1: “The ABC of Programming” (pp.11-52)
## ABC of Programing
### A
Script - list of instructions that a computers follows in order to achieve a goal set by the developer.
    - Browser may only use a certain part of the script based on how the user is interaction with the web page
        -If and event happens, then a section of code may fire in response. 
    - Programatic approaches are required for communicating with the computer. 
        - Give the coomputer a list of small tasks to complete in order to complete a larger task/goal.
    
### B
Computers make webpages with models of world situations with data programmed by developers.
- These models are made up of objects which can have properties that better explain the object. Also made up of:
    - Methods, that use the properties of an object to perform tasks. 
    - Events, that are related to the prior two. Events are triggered based on the interactions of the users.
        - (Ex. When this happens, do this)
The webpage can be made interactive by the way that the browser model in written.  
### C
#### Writing a script for a webpage
JS is a seperate file that manipulates the source code from HTML and the styling from CSS.
    - The Src code (HTML) is not ammended, but in the DOM it is rendered by JS differently. 

#### How to use objects and methods
In a script, we are going to use:
- An object "document"
- A member operator
- A method




















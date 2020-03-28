# HTML Chapter 1: “Structure” (pp.12-39)
### Summary/Things to look out for while reading 

***************
* HTML pages are text documents.
* HTML uses tage (characters that sit inside angled brackets)to give the info they surround special meaning 
    - Tags are oftenn referred tp as e;e,emts 
    -  Usually come in pairs < >
    - Opening tags carry attributes, which tell us more about the content of that element
    - Attributes require a name and a value
    - Learn where tags can go and what they are used for. 
**************
This is what an HTML structure looks like. 
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
 - Tags act as container that tell you about the content.

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
Always appear as thought they continue on the same line as their neighbors.
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
- instead of using DIV for every section of the document, we use:
```
<section>
<article>
    <figure> </figure> 


```

```
<!DOCTYPES html>
<html>
    <head>
        <title> </title>
        <style type="text/css">
        ...
        ...
        ...
        </style>
    </head>
    
    <body>
    <div class="course"
    >
    </body>
</html> 
```


//
//
************
************
************
# HTML Chapter 18: “Process & Design” (pp.452-475)

### Markdown Entry Ideas
- Blog Article (2-3 paragraphs with code sample)
- Dictionary / Flash Cards
- Notes in outline form
- Use an analogy
- Explain a detail in depth
- Use WHY, WHAT, HOW structure
- Tutorial / walk through an example as though you were teaching a 102 student
- Write a quiz
- Create a vocabulary/definition list
- Write a cheat sheet
- Create a diagram / visualization / cartoon of a topic
- Anthropomorphize the concepts, and write a conversation between them
- Build a map of the information
- Construct a fill-in-the-blank worksheet for the topic
# Read: 03 - Flexbox and Templating
[README](/README.md)

# Javascript Templating Language and Engine— Mustache.js with Node and Express 
[article](https://medium.com/@1sherlynn/javascript-templating-language-and-engine-mustache-js-with-node-and-express-f4c2530e73b2)

## mustache
logic-less templating
- there are no if or else statements, or for loops. Mustache only uses tags which can be replaced with a value, some nothing, and others a series of values.
-'mustache supports various languages, we don’t need a separate templating system on the server side.'

*Mustache is a specification for a templating language*

- need to install node and express
```
$ npm install mustache --save
```
Works in your server.js
-need to configure it for your sever.js/app.js/index.js
```
var mustacheExpress = requir('mustache-express');
// regoster '.mustache' extension with the Mustache Express
app.engine('html', mustacheExpress())

app.set('view engine', 'html');
app.set('views', _dirname + '/src/views')




Read: 03 - HTML Lists, CSS Boxes, JS Control Flow
3/31/20
## Chapter 3: “Lists” (pp.62-73)

There are Three types of lists in HTML:
- Ordered lists - each item in the list is numbered 'ol'
- Unordered lists - these begin with bullet points 'ul'
- definition lists - a set of terms along with the def for the terms 'dl'
  - 'dt' contains the term being defined
  - 'dd' used to contain the definition

  Nested Lists
  - mulitiple lists can be put in to a list

## Chapter 13: “Boxes” (pp.300-329)

X Controlling size of boxes
X Box model for borders, margin and padding 
X Displaying and hiding boxes

**Important** Css treats HTML elements as if they are in their own box
- There are bunches of different properties to change the appearance of these boxes
- Boxes have three available properties that can be manipulated:
  1. Border
    - Border width
    - border style
    - border color

    'The border property allows you to specify the width, style and color of a border in one property (and the values should be coded in that specific order).' (pg. 312)

  2. Margin
    - Controls the gap between boxes
    - Margins may overlap 
  3. Padding
    - Padding dictates how much space is between the content and the box border

Centering Content
- need to set a width for the box or it will take over the entire width
- set the margins to auto

Text-align property aligns the text inside of the box

Display:
- this property lets you change inline elements into block-level elements or vice versa. It can also hide elements. Use 'none' to do that.

You can do so much with css to boxes
- You can hide boxes
- You can give border images
- Make box-shadows
- Give rounded corners
- Make elliptical shapes

**Important** : You can make content more readable by controlling the width of the box that contains it.

## Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182) 

Switch Statements
- contain a variable called the switch value
- similar to and 'if else', each case indicates a possible value for the switch variable and the code that should run if the variable matches the value
![switchVsIf..else](img/switch-vs-if...else.png)

Type Coercion and Weak Typing 
- If  you write something that js does not expect, it will try to make it work without throwing an error.
-Weak typing refers to js not needing to know the specific data type of each variable.

Truthy and Falsy Values
- ???? I do not get this. I understand what it does in the code, but I do not understand the logic. **LOOK INTO THIS**
-can be used to check for the existence of an elemen on a page
'===' and '!==' lead to fewer unexpected values than ==and !=

#### Loops
-Check for a condition. If true, the block of code will run. It will do so until it is false.

![forloop](img/switch-vs-if...else.png)

-loop counters
  - counter tells the code to run a specified number of times.
  'var i = 0;' 'i < 10;' 'i++'

  #### All values evaluate to either truthy or falsy. 

  #### difference between while and for loops????

A for loop is often used to loop through the items in an array.




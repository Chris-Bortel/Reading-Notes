# Read: 05 - HTML Images; CSS Color & Text

# Chapter 5: “Images” (pp.94-125)
### How to add images to pages
Storing images on your site
- You will want to save the image file to a folder in your assets called images. Then you will call in your code using an img tag with the source, alternative text, and a title. ex) pp. 99
```
<img src="images/quokka.jpg" alt="A family of quokka" title="The quokka is an Australian marsupial that is similar in size to the domestic cat." />
```
### Choosing the right format
You want images to emphasize the content on the page. 
**JPEGs** are the best format to save images as. 

### Optimizing images for the web
You do not want images that are bigger or higher resolution than the average computer. That just slows down load times.
- Save inmages at the size that you plan to use that on the web page. Also save them in the appropriate format. 





******************
# Chapter 11: “Color” (pp.246-263)
Color can really make or break your site, **No One** wants to look at garbage! People want to feel things; color does that!

### How to specify colors
Three ways to specify color in CSS
- Color names
- Hex codes
- RGB values
#### examples in order pp. 249
```
/* color name */
h1 {
  color: DarkCyan;}
/* hex code */
h2 {
  color: #ee3e80;}
/* rgb value */
p{
color: rgb(100,100,90);}
```
- When in doubt, use a color picker!

### Color terminology and contrast 
Colors in computer land are all composed by different amounts of red, green, and blue mixtures. 
#### Terms to keep an eye on. 
- RGB Values
- Hex codes
- Color names
- Hue 
- Saturation
- Brightness
- Opacity

### Background color
Allows you to modify elements background colors based on their relation in place order

### Wrap up!
There are all sorts of different ways to use color in order to make your website look more appealing and perform better. 

*******************
# Chapter 12: “Text” (pp.264-299)
Manipulating text is an exciting part of putting your sense of style into your page. 
-fortunately, there are CSS properties at your finger tips that can control font, size, weight, style, and spacing.
### Size and typeface of text
- Size controlled by:
  - Pixels - Size is set regardless of screen size
  - Percentages - Responsive to screen sizes
  - EMS - Responsive to screen sizes
There are set options for fonts

### Bold, italics, capitals, underlines, AND their properties
- Bold: font-weight
- Italic: font-style
- Capitals: text transform 
- Underlines: text-decoration 
### Spacing between lines, words, and letters
This is controlled by kerning
- controling the space between each letter with the letter-spacing property pp. 284

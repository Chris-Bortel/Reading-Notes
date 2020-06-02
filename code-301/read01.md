# Read: 01 - SMACSS and Responsive Web Design



[README](/README.md)
[Shay Howe's intro to RWD](http://learn.shayhowe.com/advanced-html-css/responsive-web-design/)
Responsive Web Design
- Responsive, Adaptive, Mobile

 - Responsive generally means to react quickly and positively to any change
 - Adaptive means to be easily modified for a new purpose or situation, such as change. 
 - Mobile means to build a separate website commonly on a new domain solely for mobile users. 




Flexible Layouts
- flexible layouts, media queries, and flexible media.
  - Relative lengths - used to declare common grid property values such as width, margin, or padding.
  - Relative Viewport Lengths
    - vw: Viewports width
    - vh: Viewports height
    - vmin: Minimum of the viewport's height and width
    - vmax: Maximum of the viewport's height and width
- dont use fixed measurement units. 



Flexible Grid


Media Queries
Mobile First
Viewport
Flexible Media

# All About Floats
[Css Tricks](https://css-tricks.com/all-about-floats/)

- Floats can remove elements from the flow of the page.
- They are helpful when element sizes change. They allow the element changing to push the ajoining element aside instead of covering it. Called reflow.



Clearing floats is important
- The clear propert pushed the element below the floated property. This allows the flow of the site to not be unexpectedly jacked up.



The great collapse
- This is when the parent element of the floated element/s has no height. 
- This can be fixed by clearing the float after the floated elements in the containing element, but before the close. 



Problems with floats
- Pushdown
- Double margin
  - if you apply a margin to an element in the same direction as a float, you will end up with a double margin. Can fix it with `display:inline`
- 3px Jog
  - This is what I have been dealing with!!! I need to fix that by setting the width of the affected area.
- Bottom Margin Bug
  - When a floated parent has floated children inside. The bottom margin of those children is ignored. instead use the bottom padding on the parent.





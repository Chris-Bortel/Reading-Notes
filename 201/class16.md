# Read: 14a - CSS Transforms, Transitions, and Animations

[GitHub Repo](https://github.com/Chris-Bortel/Reading-Notes)

[Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)
Transform Syntax

```
div {
  -webkit-transform: scale(1.5);
     -moz-transform: scale(1.5);
       -o-transform: scale(1.5);
          transform: scale(1.5);
}
```
-keeping the vendor prefixes in is currently the best practice in production

## 2D Transforms
-  Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. 
  - 2D rotate can rotate that elements from 0 - 360 degrees. Positive values rotate elememt clockwise while  negative value rates the element counter clockwise.

```
HTML

<figure class="box-1">Box 1</figure>
<figure class="box-2">Box 2</figure>

CSS

.box-1 {
  transform: rotate(20deg);
}
.box-2 {
  transform: rotate(-55deg);
}

```

- Scale: scaleY scales width and scaleX scales only height of an element 
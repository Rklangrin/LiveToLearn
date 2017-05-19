

## Box-sizing properties

The default box-sizing property is **content-box**, which means the width and height properties include only the content of the element. 
  * You want to use **border-box** instead in order to include content, padding, and border (NOT margin) in the height and width properties
  
```css
 box-sizing: content-box; /* This is default property. Height and widtch include only contenct */
 box-sizing: border-box; /* Height and width include content, padding, and border */
```

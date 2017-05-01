General: 

[See my codepen for the below examples](https://codepen.io/rklangrin/pen/wddagL?editors=1100)

- The styling that is more specific will take precedent. 
- Styles cascade down. If you declare a style like `text-align: center` using a less specific selector like div, and none of the more specific selectors (maybe div.this-class) also referring to divs don't mention a text-align property, then they will still all have `text-align: center` in them. It will only be negated if a more specific selector overrides that style by putting something like `text-align: right`. 

```html
<div>1. Generic div</div>
<div class="this-class">2. One class</div>
<div class='this-class another-class'>3. Two classes</div>
<div id="id" class="this-class another-class">4. div with two classes and id</div>
```

```sass
*
  box-sizing: border-box
  
div 
  border: 1px solid red
  height: 100px
  width: 200px
  margin: 10px
  background-color: grey

#id 
  background-color: pink
  
.another-class
  background-color: blue

.this-class
  background-color: green

```

In the situation above, div 1 is grey, 2 is green, 3 is also green, and 4 is pink.
* 2 and 3 are both green, even though .another-class is coded to be blue. Since they have the same level of specificity, the one declared last in the file will take precedent. If the .another-class selector were declared after .this-class, then div 3 would be blue. 
* 4 is pink because id is more specific than class and thus takes precedent

```sass
.another-class.this-class 
  background-color blue
```

If I added more specificity to the .another-class selector as shown above, then div 3 would change to blue, no matter where it was in the file because it is now more specific by referencing both classes as opposed to just one.

### General specificity rule to figure out what styling will take precedent
**0 {id} 0 {class} 0 {tag}**
* How many ids does it have referencing it
* how many classes does it have referencing it
* how many rags does it have referencing it

100 beats 053 - meaning 1 id being referenced will take precedence over 5 classes and 3 tags

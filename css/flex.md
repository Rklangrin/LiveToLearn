# Flexbox

You can use `display: flex` on some container element and all the child elements of that container are affected. 

The different properties you can use are below:
  - **justify-content** (aligns items horizontally)
    - flex-start
    - flex-end
    - center
    - space-between
    - space-around
  - **align-items** (aligns items vertically)
    - flex-start
    - flex-end
    - center
    - baseline
    - stretch
  - **flex-direction** (defines direction items are placed in the container)
    - row
    - row-reverse
    - column
    - column-reverse
  - **order** (must be applied to individual items within the container to change the order)
    - by default, item order property has a value of 0
    - can be set to positive or negative integer value (more negative on the left, more positive on the right)
  - **align-self** (must be applied to individual items)
    - same values as align-items
  - **flex-wrap** 
    - no-wrap
    - wrap
    - wrap-reverse
  - **flex-flow** (combination of flex-direction and flex-wrap - takes two values)
  - **align-content** (set how multiple lines of items are spaced apart from each other - this is in a situation where items are wrapped onto another line)
    - flex-start
    - flex-end
    - center
    - space-between
    - space-around
    - stretch



    
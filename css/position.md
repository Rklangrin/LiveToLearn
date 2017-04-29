Position:
  * Absolute - you tell the element absolutely where on the page it should be. 
    * if absolute, you must give it top, right, left, or bottom descriptions to say where from the edge of the page you want it to be. 
    ex: 

    ```css
      p {
        position: absolute;
        top: 0px;
        right: 0px;
      }
      /* The above element will now be located at the top right of the screen because it is 0 pixels away from the top and 0 pixels away from the right side of the screen. */
    ```
  * Fixed - with relation to your viewport (the screen that you see on your browser) the element is now 'fixed.' If you scroll or move the page right or left, the element will stay in the same location.  
  * Relative - This changes the location of the element from where it would organically wind up on the page.
## Variable declarations - let vs. const

const:
  * block scope
  * the variable identifier cannot be reassigned. Once you assign it, you can no longer change the variable. HOWEVER, you can change the data the variable holds. 
    * For instance, if it's an object saved in a variable, the object properties can change, but the variable will always point to that same object. 

let:
  * block scope
  * cannot redeclare a let variable within the same scope, BUT you can reassign it. 
  * The code below is acceptable:
  ```javascript
    let count = 0;
    count = 5;
  ```

## Arrow Functions
- cannot be used as constructors

```javascript
  let numbers = [1, 2, 3, 4, 5];

  let evenNumbers = numbers.map(num => num * 2);
  // parentheses are optional when there is only one parameter name (num in this case)

  // this is equivalent to saying:
  evenNumbers = numbers.map(function(num){
    return num * 2;
  })
```
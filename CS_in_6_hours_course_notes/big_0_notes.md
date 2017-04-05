# Big O
This is a method for analyzing how efficient an algorithm is. Big O is also referring to the worse possible scenario that the algorithm could be used for. See below.  

Example 1: Linear search
```javascript
function find(needle, haystack) {
  for (var i = 0; i < haystack.length; i++){
    if (haystack[i] === needle) {
    return true;
    }
  }
}
```

This function has a Big-O of n. Why? Consider if the "needle" was the last element in the haystack array. The 'for loop' would have to go through each element in the array before it found the needle - meaning the loop would run n times (n = number of items in haystack array). Therefore, Big-O in this example is n. 

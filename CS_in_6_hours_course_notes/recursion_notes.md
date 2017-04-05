# Recursion

In computer science, this is just when a function calls itself. See example below in ruby. The example function will take a positive integer, n, and return the nth number in the fibonacci sequence. The fibonacci sequence is a series of numbers where each number is a sum of the two numbers before it, and the sequence starts with 1 and 1. THe next (3rd) number is 2 because 1+1 = 2. The next (4th) number is 3 because 2 + 1 = 3, and so on. 

fibonacci sequence: 1, 1, 2, 3, 5, 8, 13, 21, ...

```ruby
def find_nth_fibonacci_number(n)
  return 1 if n <= 2
  find_nth_fibonacci_number(n-1) + find_nth_fibonacci_number(n-2)
end

# ruby has implicit return, meaning the last line of a method will be the return value even if you don't explicitly type return.
```

The first line in any recursive function is generally going to be the base case (sometimes there is more than one base case as you can see above). The base case is when you stop recursing. If you don't have a base case then the function will never stop calling itself. In the example above, the recursion stops when the number being inputted into the function is equal to 1 or 2. 

The code above is short and easy to read. The problem with it is when it's being called for the 20th number in the sequence. That number ends up being 6765. This means we added 1 to itself 6765 times. In this case, you are sacrificing readability for efficiency. The problem could be done more efficiently with iteration. 


* Each level of a recursive call can maintain it's own state.  
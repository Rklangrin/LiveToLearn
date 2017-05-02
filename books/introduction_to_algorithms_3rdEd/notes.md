# Algorithms

* A sequence of computational steps that transforms some input into the output. 
* Algorithms are efficient in terms of space and time. 
  * space refers to the memory available 
  * time refers to the amount of time it takes for the computer to run the algorithm.

** Parallelism **
 * computers are designed to contain several processing cores that function in parallel to one another. Because of this, algorithms need to be designed with parallelism in mind in order to best utilize a computer's multi-core processor.

** Space Complexity **
  * measure of how much memory the algorithm takes up

** Time complexity **
  * measure of how much time the algorithm takes to complete


## Analyzing Algorithms
Primitive Operations - each of the following instructions takes a constant amount of time.  
  * arithmetic - add, subtract, multiply, divide, remainder, floor, ceiling
  * data movement - load, store, copy
  * control flow - conditional branch, subroutine call and return

Input size - this often depends on the problem. It could refer to: 
  * number of items in the input (most common for sorting)
  * total number of bits needed to represent input (used for multiplying two integers)
  * two numbers referring to vertices and edges in a graph (if algorithm input is a graph)

Running Time - the number of primitive operations that need to be executed. 
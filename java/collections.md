# Collections

![alt text](http://www.programcreek.com/wp-content/uploads/2009/02/java-collection-hierarchy.jpeg "Logo Title Text 1")

## Arrays
* Array size is **fixed** upon initialization. 
* Arrays are **zero-based**
* **length** is an attribute of all arrays 

declaration examples:
```java
  int[] integers = new int[5];

  int[] integers = new int[] {1, 2, 3, 4, 5};

  int[] integers = {1, 2, 3, 4, 5};
```

you can type integers[1] to get the value at index 1 in the array. 

## Lists
* Ordered collection, a.k.a. 'sequence'
* Can only hold objects of a specified type
* **size** is an attribute of all lists, which is basically the same as .length

declaration examples:
```java
  List<String> listOfStrings = new ArrayList<String>();

  List<String> listOfStrings = new ArrayList<>();
```

**Methods:**
* .add( ) -- Similar to .push
* .get(x) -- This is accessing an element in the list at index = x.
* .get(x, y) -- This will place the value of y at the index of x in the array. 

## Sets
* each element in a set must be unique.
* Can only hold objects
* Elements in a set do not maintain any order.

declaration examples:
```java
    Set<Integer> setOfIntegers = new HashSet<Integer>();
    setOfIntegers.add(Integer.valueOf(10));
```

### Array Lists

Pros:
* Fast random read access. Grab any element in the list by using it's index

Cons:
* Adding or removing anywhere but the end requires shifting of every other element in the array after the location it was added
  * I.e. if you have an array of 10 values and want to add an element to the 2nd spot (index = 1) in the array, then the next 8 spots all have to be shifted over one. 
* If you add more elements than the array can hold, then what happens is a new array (1.5 times bigger) is created and the old array is copied into it. 


### Linked Lists

Pros:
* Constant-time insertions/removals

Cons:
* Searching for item in list takes time proportional to size of list
* Takes up more memory than ArrayLists because at each location in the list, memory needs to be allocated for the pointer to the next item and a pointer to the previous item in the list.
  * However, ArrayLists are static so when you create an array, you set aside memory for however many spaces you want in the array, even if you don't fill them up right away.

declaration example:
```java
  LinkedList<String> linkedlist = new LinkedList<String>();
```

Useful Methods:
  * .add("item") - adds item to end of the list
    * .addFirst() - adds item to beginning of list
    * .addLast()
  * .set(index, "item")
  * .get(index)
  * .remove("item")
    * .remove(index) 
    * .removeFirst()
    * .removeLast()


## Maps
* Similar to a ruby hash, these are collections that store key-value pairs. 
* Keys must be unique. 
* Can only hold objects

declaration examples:
```java
  Map<String, Integer> mapOfIntegers = new HashMap<>();
  mapOfIntegers.put("1", Integer.valueOf(1));

  // Retrieve a value by using the key
  mapOfIntegers.get("1");
```

You can create a set of the keys of a map like so:
```java
  Set<String> keys = mapOfIntegers.keySet();

  // now you can iterate through all the Map values by iterating through the created set, 'keys'
```

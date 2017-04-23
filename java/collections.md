# Collections

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

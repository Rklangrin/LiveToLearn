Primitive Data Types:

* Boolean (defaults to false)     
  * Class: java.lang.Boolean
* Byte - 8 bits
  * Class: java.lang.Byte
* Char - 16 bits
  * Class: java.lang.Character
* Short - 16 bits
  * Class: java.lang.Short
* Int - 32 bits
  * Class: java.lang.Integer
* Long - 64 bits
  * Class: java.lang.Long
* Float - 32 bits
  * Class: java.lang.Float
* Double - 64 bits
  * Class: java.lang.Double

Each of these primitive data types have a corresponding object wrapper class. So you can convert an int to an Inteer object, or a double to a Double object. 
  * Going from primitive to object is called "boxing"
  * THe opposite is called "unboxing"

Example:
```java
  int value = 238;
  Integer boxedValue = Integer.valueOf(value);

  // This has just changed the int primitive datatype to an object from the Integer class. Now it can be stored in an ArrayList, which can only store objects.
```

Apparently an Integer is different than an int. 

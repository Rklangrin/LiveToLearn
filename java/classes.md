# Classes
- convention to name classes using CamelCase.
- class names only have letters and numbers

Classes have two types of members: Variables and Methods. 

## Variables
- a.k.a. instance variables. 
Variables have: 
  - assessSpecifier (public, protected, private, 'no specifier')
  - dataType
  - variableName
  - initialValue (optional)


Possible AsessSpecifier values are:
  - public: Any object in any package can see the variable 
    - * Generally a bad idea to use public variables * 
  - protected: any object in the same package, or in a subclass, can see the variable
  - No specifier: only objects in the same package can see the variable. 
  - Private: Only the class containing the variable can see it. 

  ## Methods
  - Constructor methods are used only to create an instance of the class. 
    - Constructors are optional and if you don't use one, then the compiler provides one for you (but it doesn't initialize any instance variables). 
    - Name of constructor must match the name of the class

  The constructor method is defined inside of the class. 

Other methods: 
  Conventions:
  1. Start with lowercase letter
  2. Avoid numbers unless absolutely necessary
  3. Use only alphabetic chars.

Static Methods - Class methods
Instance methods - These are methods of the object that is an instance of a class. 
# Object-Oriented Programming Concepts

## What Is an Object?

any thing have a state and bhavior is an object.


### Bundling code into individual software objects provides a number of benefits, including:

Bundling code into individual software objects provides a number of benefits, including:

1. Modularity: The source code for an object can be written and maintained independently of the source code for other objects.

2. Information-hiding: By interacting only with an object's methods, the details of its internal implementation remain hidden from the outside world.

3. Code re-use: If an object already exists  you can use that object in your program.

4. Pluggability and debugging ease: If a particular object turns out to be problematic, you can simply remove it from your application and plug in a different object as its replacement. 

## What Is a Class?

anything ahd the same used conseder like a class



## What Is Inheritance?

its the same information or behaveor between two differant object


## What Is an Interface?

objects define their interaction with the outside world through the methods that they expose.

## What Is a Package?

 package is a namespace that organizes a set of related classes and interfaces. 



 ## Interfaces in Java

 In the Java programming language, an interface is a reference type, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types.


## Inheritance

Definitions: A class that is derived from another class is called a subclass 

A subclass inherits all the members (fields, methods, and nested classes) from its superclass


### What You Can Do in a Subclass?

A subclass inherits all of the public and protected members of its parent, no matter what package the subclass is in. If the subclass is in the same package as its parent, it also inherits the package-private members of the parent.

* The inherited fields can be used directly, just like any other fields.
* You can declare a field in the subclass with the same name as the one in the superclass, thus hiding it (not recommended).
* You can declare new fields in the subclass that are not in the superclass.
* The inherited methods can be used directly as they are.
* You can write a new instance method in the subclass that has the same signature as the one in the superclass, thus overriding it.
* You can write a new static method in the subclass that has the same signature as the one in the superclass, thus hiding it.
* You can declare new methods in the subclass that are not in the superclass.
* You can write a subclass constructor that invokes the constructor of the superclass, either implicitly or by using the keyword super.

## Private Members in a Superclass

A subclass does not inherit the private members of its parent class. 


## Casting Objects

asting shows the use of an object of one type in place of another type, among the objects permitted by inheritance and implementations.



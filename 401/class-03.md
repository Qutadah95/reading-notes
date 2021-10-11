# Java Primitives versus Objects

## Java Type System

we have two main type of system: 

1. autoboxing : like  Integer j = 1; 

2. unboxing : like int i = new Integer(1);

## Pros and Cons

1. Single Item Memory Footprint : 

 the primitive type take from the memory : 

* boolean – 1 bit
* byte – 8 bits
* short, char – 16 bits
* int, float – 32 bits
* long, double – 64 bits

Boolean type take from the memory : 

* Boolean – 128 bits
* Byte – 128 bits
* Short, Character – 128 bits
* Integer, Float – 128 bits
* Long, Double – 192 bits


2. Memory Footprint for Arrays : 


single-element arrays of primitive types are almost always more expensive (except for long and double) than the corresponding reference type.

3. Performance : 

the java code depends on very much on the hardware on which the code runs 

4. Default Values : 

Default values of the primitive types are 0 

##  Usage 

the primitive types are much faster and require much less memory

## Conclusion : 

we should try to use the primitive type because its faster in run

# Exceptions

## What Is an Exception?

An exception is an event that occurs during the execution of a program that disrupts the normal flow of instructions.

## The Catch or Specify Requirement 

we have three Kinds of Exceptions : 

1. the checked exception.

2. the error 

3. the runtime exception


## The try-with-resources Statement 

its the same in js we put the try {

    all the code

}catch{


    an error

}

# Scanning

## Breaking Input into Tokens

a scanner uses white space to separate tokens

## Translating Individual Tokens

The ScanXan example treats all input tokens as simple String values.Scanner also supports tokens for all of the Java language's primitive types (except for char).










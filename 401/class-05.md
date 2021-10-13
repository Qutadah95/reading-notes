# Big O: Analysis of Algorithm Efficiency

its describ the efficiency and that have two baiced : 

1. Running Time

2. Memory Space

## Overview

we have 4 factor to consider which is : 

1. Input Size : its debend on the size of the input

2. Units of Measurement : To evaluate a function for Time and Space complexity 

3. Orders of Growth : we will descibe the efficiency by using N 

4. Best Case, Worst Case, and Average Case : 

* Worst Case:  the worst input of size n

* Best Case:  the best input of size n

* Average Case:  a “typical” or “random” input of size n.


# Linked Lists

## What is a Linked List

A Linked List is a sequence of Nodes that are connected/linked to each other and we have tow type of linked : 

* Singly

* Doubly

## What does it look like

This is what a Singly Linked List looks like

## Terminology:

1. Linked List : A data structure that contains nodes that links
2. Singly - Singly : refers to the number of references the node has
3. Doubly - Doubly : refers to there being two (double) references within the node
4. Node - Nodes : the individual items/links that live in a linked list
5. Next - Each : ode contains a property called Next
6. Head - The Head : is a reference of type Node to the first node in a linked list.
7. Current - The Current : is a reference of type Node to the node that is currently being looked at . 

## Traversal

we dont use for each loop but we use while loop to do it.

## Traversal Big O

The Big O of time for Includes would be O(n). 

## Adding a Node

### Adding O(1)

Order of operations is extremely important when it comes to working with a Linked List.


## Print Out Nodes

Printing out all of the nodes in a Linked List is very similar to what we did in the Includes() method. This is because we are leveraging our Current node and a while loop to traverse through the existing linked list.

## Prerequisites

When making your Node class, consider requiring a value to be passed in to require that each node has a value.

# What’s a Linked List, Anyway?

one of the imbortant things is choose the way to orignize the information 

## Linear data structures

whene the information comming in the same line called liner data structures

## Memory management

array need a contiguous block of memory

linked list dont need to be contiguous in memory. they can grow dynamically

## Parts of a linked list

 A linked list is made up of a series of nodes, which are the elements of the list.

 head => node => node => node => null 

 one node is made up of 2 part : some data thats it hold and reference to the next node 



 ## Different types of linked list :

1. singly linked list 

2. doubly linked list

3. circular linked list

## There are two major points to consider when thinking about how an algorithm performs:

given how much time and memory it needs.


First, we find the head node of the linked list.
Next, we’ll make our new node, and set its pointer to the current first node of the list.
Lastly, we rearrange our head node’s pointer to point at our new node.

But inserting an element at the end of a linked list is a different story.

1. Find the node we want to change the pointer of (in this case, the last node)
2. Create the new node we want to insert and set its pointer (in this case, to null)
3. Direct the preceding node’s pointer to our new node

## When to use an array versus a linked list


array :
* inserting and deleting can be really slow
* searching is fast
* static and fixed size , not as easy to qrow or shrink
* allocates memory when created,a contiguous chunk of resources,even if all of that space isnt filled 
* finding elemant is fast and since arrays are index and use cantiguoos memory binary search is an option
=> helpful if you do know the size of the list you need random acsess to elemant or want to iterate guickly

linked list :

* inserting and deleting can be really fast
* searching is slow
* dunamic size can grow and shrink easily
* only allocates vesources as required at run time using non - contiguous thunks of memory as needed
* finding elements requires travevsal and travsal is slow since you cant use binary search
=> helpful if you dont know the size of the list and mostly want to add or remove things quiekly without random acsess










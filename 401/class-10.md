# Stacks and Queues

## What is a Stack ?

A stack is a data structure that consists of Nodes.

## Common terminology for a stack is : 

1. Push 
2. Pop 
3. Top
4. Peek 
5. IsEmpty 

## Stacks follow these concepts :

1. FILO : first in last out 
2. LIFO : Last In First Out


## Push O(1) : to push a new node

to you can do a push to the stack you need to : 

1. have a node (creat a one)

2. have next not = null ( assign the next)

3. stack.push now your new node pushed .


## Pop O(1) : to remove a node 

1. creat a referance called temp for the top node 

2. re-assign top to the value that the next property is referencing

3. stack.pop now the node is deleted


## Peek O(1) : will only be inspecting the top Node of the stack

1. alograthem peek(){

    return top.value
}


## IsEmpty O(1) : when the seack empty return true

1. algorathem isEmpty(){

    return top = null
}


the big O's for the time is one for all of them



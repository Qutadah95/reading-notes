# Android Tasks and the Back Stack

## Tasks and the back stack 

A task is a collection of activities that users interact with when trying to do something in your app

## Lifecycle of a task and its back stack


When the current activity starts another, the new activity is pushed on the top of the stack and takes focus. The previous activity remains in the stack, but is stopped. When an activity stops, the system retains the current state of its user interface. When the user performs the back action, the current activity is popped from the top of the stack and the previous activity resumes .

## Background and foreground tasks

if i have x , y activity if x run in the foreground then the y run in the background and the oppesite is true

## Multiple activity instances

run the same activity multitime in the background

## Lifecycle recap


* When Activity A starts Activity B, Activity A is stopped, but the system retains its state
* When the user leaves a task using the Home button or gesture, the current activity is stopped and its task goes into the background. 
* If the user presses or gestures Back, the current activity is popped from the stack and destroyed.
* This behavior is different for root launcher activities when your app is running on a device that runs Android 12 or higher.
* Activities can be instantiated multiple times, even from other tasks.

## Manage tasks

> You can do these things and more, with attributes in the <activity> manifest element and with flags in the  
> intent  that you pass to startActivity().

## Defining launch modes

by using : 

1. Using the manifest file

2. Using Intent flags

## Define launch modes using the manifest file

The launchMode attribute specifies an instruction on how the activity should be launched into a task: 

1. standard
2. singleTop
3. singleTask
4. singleInstance

## Clear the back stack

There are some activity attributes that you can use to modify this behavior:

* alwaysRetainTaskState
* clearTaskOnLaunch
* finishOnTaskLaunch



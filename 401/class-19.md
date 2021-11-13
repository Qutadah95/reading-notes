# Android fundamentals


## Application Fundamentals

we can use c++ , java or Kotlin to write android app .

An Android package, which is an archive file with an .apk suffix, contains the contents of an Android app that are required at runtime and it is the file that Android-powered devices use to install the app.

Each Android app lives in its own security sandbox, protected by the following Android security features:

* The Android operating system is a multi-user Linux system in which each app is a different user.
* By default, the system assigns each app a unique Linux user ID
*  Each process has its own virtual machine (VM), so an app's code runs in isolation from other apps.

there are ways for an app to share data with other apps and for an app to access system services:

* It's possible to arrange for two apps to share the same Linux user ID
* An app can request permission to access device data such as the device's location, camera, and Bluetooth connection


## App components

There are four different types of app components:

1. Activities : 

An activity is the entry point for interacting with the user.

An activity facilitates the following key interactions between system and app:

* Keeping track of what the user currently cares about  to ensure that the system keeps running the process that is hosting the activity.

*  thus more highly prioritized keeping those processes around.

* Helping the app handle having its process killed so the user can return to activities with their previous state restored.

* Providing a way for apps to implement user flows between each other


2. Services

A service is a general-purpose entry point for keeping an app running in the background for all kinds of reasons

Started services tell the system to keep them running until their work is completed 

3. Broadcast receivers

A broadcast receiver is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements


4. Content providers

A content provider manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access


## Activating components

by using An intent object .


## The manifest file

the app must declare all its components in AndroidManifest.xml, which must be at the root of the app project directory.

## Declaring components

 > <activity> elements for activities.
> <service> elements for services.
> <receiver> elements for broadcast receivers.
> <provider> elements for content providers.

## Declaring component capabilities

> we can declare an intent filter for your component by adding an
>  <intent-filter> element as a child of the components declaration element.

## Declaring app requirements

declare the android version for the app and choose it for the app 



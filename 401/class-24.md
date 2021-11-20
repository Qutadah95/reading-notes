# Espresso

Use Espresso to write concise, beautiful, and reliable Android UI tests.

Espresso tests state expectations, interactions, and assertions clearly without the distraction of boilerplate content, custom infrastructure, or messy implementation details getting in the way.


## Synchronization capabilities

Each time your test invokes onView(), Espresso waits to perform the corresponding UI action or assertion until the following synchronization conditions are met:

* The message queue is empty.
* There are no instances of AsyncTask currently executing a task.
* All developer-defined idling resources are idle.

This capability gives you more reliable and dependable test results.

## Packages

* espresso-core - Contains core and basic View matchers, actions, and assertions. 
* espresso-web - Contains resources for WebView support.
* espresso-idling-resource - Espresso's mechanism for synchronization with background jobs.
* espresso-contrib - External contributions that contain DatePicker, RecyclerView and Drawer actions, accessibility checks, and CountingIdlingResource.
* espresso-intents - Extension to validate and stub intents for hermetic testing.
* espresso-remote - Location of Espresso's multi-process functionality.

## Create UI tests with Espresso Test Recorder 

1. Turn off animations on your test device 
2. Record an Espresso test
3. Record UI interactions
4. Add assertions to verify UI elements
5. Save a recording
6. Run an Espresso test locally
7. Run an Espresso test with Firebase Test Lab for Android

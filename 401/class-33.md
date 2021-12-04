# Intent Filters

## Allowing Other Apps to Start Your Activity 

If your app can perform an action that might be useful from another app, your app should be prepared to respond to action requests by specifying the appropriate intent filter in your activity.

## Add an Intent Filter

In order to properly define which intents your activity can handle, each intent filter you add should be as specific as possible in terms of the type of action and data the activity accepts.

The system may send a given Intent to an activity if that activity has an intent filter fulfills the following criteria of the Intent object:

1. Action
2. Data
3. Category

## Handle the Intent in Your Activity

In order to decide what action to take in your activity, you can read the Intent that was used to start it.

As your activity starts, call getIntent() to retrieve the Intent that started the activity.

## Return a Result

If you want to return a result to the activity that invoked yours, simply call setResult() to specify the result code and result Intent. When your operation is done and the user should return to the original activity, call finish() to close (and destroy) your activity.


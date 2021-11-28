# Amplify and Cognito

The Amplify Auth category provides an interface for authenticating a user.and The Amplify CLI helps you to create and configure the auth category with an authentication provider.

Prerequisites

at least Android SDK API level 16 with Amplify libraries integrated

## Configure Auth Category

To start provisioning auth resources in the backend, go to your project directory and execute the command:

> amplify add auth


To push your changes to the cloud, execute the command:

> amplify push


## Install Amplify Libraries

Add the following dependency to your app's build.gradle along with others you added above in Prerequisites and click "Sync Now" when prompted:

>     implementation 'com.amplifyframework:aws-auth-cognito:1.30.0'

## Initialize Amplify Auth

Add the Auth plugin before calling Amplify.configure. Update the code you added in Prerequisites:

> Amplify.addPlugin(new AWSCognitoAuthPlugin());

> Amplify.configure(getApplicationContext());


## Check the current auth session

We can now check the current auth session.

For testing purposes, you can run this from your MainActivity's onCreate method.

>Amplify.Auth.fetchAuthSession(
 >   result -> Log.i("AmplifyQuickstart", result.toString()),
 >   error -> Log.e("AmplifyQuickstart", error.toString())
> );





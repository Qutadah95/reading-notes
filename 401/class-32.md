# Amplify and Kinesis

## Getting started

The Analytics category enables you to collect analytics data for your App. The Analytics category comes with built-in support for Amazon Pinpoint and Amazon Kinesis.

you should have a aws account 

## Set up Analytics backend

Run the following command in your project's root folder. The CLI will prompt configuration options for the Analytics category such as Amazon Pinpoint resource name and analytics event settings.

> amplify add analytics

answer this qustion : 

> ? Select an Analytics provider (Use arrow keys)
>   `Amazon Pinpoint`
> ? Provide your pinpoint resource name:
>    `yourPinpointResourceName`
> ? Apps need authorization to send analytics events. Do you want to allow guests and unauthenticated users to  
>  send  analytics events? (we recommend you allow this when getting started)
>    `Yes`

To deploy your backend, run:

> amplify push

## Initialize Amplify Analytics

> Amplify.addPlugin(new AWSCognitoAuthPlugin());
> Amplify.addPlugin(new AWSPinpointAnalyticsPlugin(this));

## Record events

> AnalyticsEvent event = AnalyticsEvent.builder()
>     .name("PasswordReset")
>    .addProperty("Channel", "SMS")
>     .addProperty("Successful", true)
>     .addProperty("ProcessDuration", 792)
>     .addProperty("UserAge", 120.3)
>    .build();

> Amplify.Analytics.recordEvent(event);

## View Analytics console

> amplify console analytics

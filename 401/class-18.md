# Using WebSocket to build an interactive web application

## Starting with Spring Initializr

we can use the [pre-initialized project ](https://start.spring.io/) to set up the project and we should use in Dependencies and select Websocket.

## Adding Dependencies

on gradle we should add this Dependencies : 

> implementation 'org.webjars:webjars-locator-core'
> implementation 'org.webjars:sockjs-client:1.0.2'
> implementation 'org.webjars:stomp-websocket:2.3.3'
> implementation 'org.webjars:bootstrap:3.3.7'
> implementation 'org.webjars:jquery:3.1.1-1'

that exiset in build.gradle

## Create a Resource Representation Class

now we create your STOMP message service.

The service will accept messages that contain a name in a STOMP message whose body is a JSON object.

## Create a Message-handling Controller

up the class use 
> @Controller

up the function use 
> @MessageMapping("")
> @SendTo("")
and return the modle name with the massege


## Configure Spring for STOMP messaging

now evrything is set so we can configure Spring to enable WebSocket and STOMP messaging.

## Create a Browser Client

now the server is set we can work on client side by create an html file , This HTML file imports the SockJS and STOMP javascript libraries that will be used to communicate with our server through STOMP over websocket



## Make the Application Executable

spring Boot creates an application class for you. 

## Build an executable JAR

we can run the application from the command line with Gradle

## Test the service

finally test the service by go to 

>  http://localhost:8080

and click the Connect button.




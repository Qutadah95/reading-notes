# Spring

## Serving Web Content with Spring MVC

### What we Will Build

we will bulid an static application and accept HTTP GET requests at: http://localhost:8080/greeting



## What You Need 

we need :

* About 15 minutes

* A favorite text editor or IDE

* JDK 1.8 or later

*  Gradle 4+ or Maven 3.2+

You can also import the code straight into your IDE:

* Spring Tool Suite (STS)

* IntelliJ IDEA

## Starting with Spring Initializr


You can use this [pre-initialized](https://start.spring.io/ ) project and click Generate to download a ZIP file. This project is configured to fit the examples in this tutorial. or do it manually 


## Create a Web Controller

controller is the unit that handle with HTTP requesest .

## Spring Boot Devtools

spring boot advantiges :

* Enables hot swapping.

* Switches template engines to disable caching.

* Enables LiveReload to automatically refresh the browser.

* Other reasonable defaults based on development instead of production.

## Run the Application

The Spring Initializr creates an application class for you.

## Build an executable JAR

by using gradle or Maven we can run the applecation

run by using gradle : 

> ./gradlew bootRun

run by using maven : 

> ./mvnw spring-boot:run

## Test the Application


Now that the web site is running, visit http://localhost:8080/greeting, and we will see the result.


## Spring MVC and Thymeleaf: how to access data from templates

In a typical Spring MVC application, @Controller classes are responsible for preparing a model map with data and selecting a view to be rendered.


the defined variables available to expressions executed in templates:

1. Spring model attributes 

2. Request parameters 

3. Session attributes 

4. ServletContext attributes

5. Spring beans


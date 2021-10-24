# Spring RequestMapping

## RequestMapping Basics

mapping an HTTP request to a method using some basic criteria using 

1. @RequestMapping — by Path 
2. @RequestMapping — the HTTP Method  



## RequestMapping and HTTP Headers

The mapping can be narrowed even further by specifying a header for the request:

1. @RequestMapping With the headers Attribute 
2. @RequestMapping Consumes and Produces 


## RequestMapping With Path Variables

1. Single @PathVariable
2. Multiple @PathVariable
3. @PathVariable With Regex

## RequestMapping With Request Parameters

## RequestMapping Corner Cases

1. @RequestMapping — Multiple Paths Mapped to the Same Controller Method
2. @RequestMapping — Multiple HTTP Request Methods to the Same Controller Method
3. @RequestMapping — a Fallback for All Requests
4. Ambiguous Mapping Error

## New Request Mapping Shortcuts

Spring Framework  all based on @RequestMapping:

* @GetMapping

* @PostMapping

* @PutMapping

* @DeleteMapping

* @PatchMapping

## Spring Configuration


# Accessing Data with JPA

## Starting with Spring Initializr

we can use this [pre-initialized](https://start.spring.io/) project and click Generate to download a ZIP file.

## Define a Simple Entity

we store objects, each annotated as a JPA entity.

## Create Simple Queries

Spring Data JPA focuses on using JPA to store data in a relational database. 

## Create an Application Class

Spring Initializr creates a simple class for the application.

## Build an executable JAR

by using Gradle or Maven.

# CrudRepository, JpaRepository, and PagingAndSortingRepository in Spring Data

## Spring Data Repositories

Each of these defines its own functionality:

* CrudRepository provides CRUD functions
* PagingAndSortingRepository provides methods to do pagination and sort records
* JpaRepository provides JPA related methods such as flushing the persistence context and delete records in a batch

## CrudRepository

the typical CRUD functionality:

* save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
* findOne(…) – get a single entity based on passed primary key value
* findAll() – get an Iterable of all available entities in database
* count() – return the count of total entities in a table
* delete(…) – delete an entity based on the passed object
* exists(…) – verify if an entity exists based on the passed primary key value

## PagingAndSortingRepository

we create a Pageable object with certain properties and we've to specify at least:

1. Page size
2. Current page number
3. Sorting

## JpaRepository


## Downsides of Spring Data Repositories

there are some basic downsides of directly depending on these as well:

* we couple our code to the library and to its specific abstractions, such as `Page` or `Pageable`; 
* by extending e.g. CrudRepository, we expose a complete set of persistence method at once. 


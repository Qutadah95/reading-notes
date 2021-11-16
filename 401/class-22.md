# Room

## Save data in a local database using Room   

The most common use case is to cache relevant pieces of data so that when the device cannot access the network, the user can still browse that content while they are offline.

 Room provides the following benefits:

 * Compile-time verification of SQL queries.
 * Convenience annotations that minimize repetitive and error-prone boilerplate code.
 * Streamlined database migration paths.

 ## Primary components

 1. The database class that holds the database and serves as the main access point for the underlying connection to your app's persisted data.
2. Data entities that represent tables in your app's database.
3. Data access objects (DAOs) that provide methods that your app can use to query, update, insert, and delete data in the database.

## Defining data using Room entities 

When you use the Room persistence library to store your app's data, you define entities to represent the objects that you want to store. 

## Anatomy of an entity

You define each Room entity as a class that is annotated with @Entity.

By default, Room uses the class name as the database table name

## Define a primary key

Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table.

## Define a composite primary key

If you need instances of an entity to be uniquely identified by a combination of multiple columns, you can define a composite primary key by listing those columns in the primaryKeys property of @Entity:

## Provide table search support

* Support full-text search

* Index specific columns

## Define relationships between objects 

Because SQLite is a relational database, you can define relationships between entities.

### Two possible approaches

we have two type : 

1. Intermediate data class

2. Multimap return types

## relationships

* one-to-one
* one-to-many
* many-to-many
* nested relationships : you might need to query a set of three or more tables that are all related to each other. In that case, you would define nested relationships between the tables.













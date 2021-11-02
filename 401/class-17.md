# Hibernate Many to Many

## A Typical Example

any given employee can be assigned to multiple projects and a project may have multiple employees working for it, leading to a many-to-many association between the two.

## Database Setup

after create a database we should create table inside the database for each one employee and projects and define the relation between them

## The Model Classes

class should refer to each other

we have : 
@ManyToMany : to create the many-to-many relationship between the entities

@JoinTable : The @JoinTable is used to define the join/link table

 @JoinColumn : The @JoinColumn annotation is used to specify the join/linking column with the main table

## Execution

tables with sample data representing the relationship.





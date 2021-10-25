# Working with Relationships in Spring Data REST

relationships between entities in Spring Data REST.


## One-to-One Relationship

1. The Data Model :

*  two entity classes Library and Address having a one-to-one relationship
*  We must be careful to have different names for each association resource

2. The Repositories : Before we create an association, sending a GET request to this endpoint will return an empty object.
3. Creating the Resources : After persisting both instances, we can establish the relationship by using one of the association resources.
4. Creating the Associations


## One-to-Many Relationship

1. The Data Model
2. The Repository
3. The Association Resources

## Many-to-Many Relationship

1. The Data Model
2. The Repository
3. The Association Resources


## Testing the Endpoints With TestRestTemplate

1. Testing the One-to-One Relationship
2. Testing the One-to-Many Relationship
3. Testing the Many-to-Many Relationship


# Integration Testing in Spring

## Preparation

## Spring MVC Test Configuration

1. Enable Spring in Tests with JUnit 5
2. The WebApplicationContext Object
3. Mocking Web Context Beans
4. Verify Test Configuration

## Writing Integration Tests

1. Verify View Name
2. Verify Response Body
3. Send GET Request With Path Variable
4. Send GET Request With Query Parameters
5. Send POST Request

## MockMvc Limitations

 because Spring prepares a fake web application context to mock the HTTP requests and responses, it may not support all features of a full-blown Spring application.

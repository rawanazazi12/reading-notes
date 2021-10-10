# What I've Learned at the 11th lecture of 401 code...

## Spring RequestMapping

1. @RequestMapping.

   The annotation is used to map web requests to Spring Controller methods.


2. @RequestMapping Basics

   - @RequestMapping — by Path

   - @RequestMapping — the HTTP Method : The HTTP method parameter has no default. So, if we don't specify a value, it's going to map to any HTTP request.


3. RequestMapping and HTTP Headers

   - @RequestMapping With the headers Attribute

   - @RequestMapping Consumes and Produces : Mapping media types produced by a controller method is worth special attention.


4. RequestMapping With Path Variables                 
   Parts of the mapping URI can be bound to variables via the @PathVariable annotation.

  - Single @PathVariable

  - Multiple @PathVariable

  - @PathVariable With Regex : Regular expressions can also be used when mapping the @PathVariable.


5. RequestMapping With Request Parameters

6. RequestMapping Corner Cases


## Accessing Data with JPA

#### Starting with Spring Initializr

 You can use this pre-initialized project and click Generate to download a ZIP file. This project is configured to fit the examples in this tutorial.

 To manually initialize the project:

 1. Navigate to https://start.spring.io. This service pulls in all the dependencies you need for an application and does most of the setup for you.

 2. Choose either Gradle or Maven and the language you want to use. This guide assumes that you chose Java.

 3. Click Dependencies and select Spring Data JPA and then H2 Database.

 4. Click Generate.

 5. Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.



## CrudRepository, JpaRepository, and PagingAndSortingRepository in Spring Data

  - CrudRepository : provides CRUD functions
  - PagingAndSortingRepository : provides methods to do pagination and sort records
  - JpaRepository : provides JPA related methods such as flushing the persistence context and delete records in a batch


### The typical CRUD functionality:

  1. save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
  2. findOne(…) – get a single entity based on passed primary key value
  3. findAll() – get an Iterable of all available entities in database
  4. count() – return the count of total entities in a table
  5. delete(…) – delete an entity based on the passed object
  6. exists(…) – verify if an entity exists based on the passed primary key value




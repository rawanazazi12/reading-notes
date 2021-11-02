# Room

### Save data in a local database using Room

 The Room persistence library provides an abstraction layer over SQLite to allow fluent database access while harnessing the full power of SQLite. In particular, Room provides the following benefits:
   - Compile-time verification of SQL queries.
   - Convenience annotations that minimize repetitive and error-prone boilerplate code.
   - Streamlined database migration paths.


### Setup
To use Room in your app, add the following dependencies to your app's build.gradle file:
   dependencies {
    def room_version = "2.3.0"

    implementation "androidx.room:room-runtime:$room_version"
    annotationProcessor "androidx.room:room-compiler:$room_version"

    // optional - RxJava2 support for Room
    implementation "androidx.room:room-rxjava2:$room_version"

    // optional - RxJava3 support for Room
    implementation "androidx.room:room-rxjava3:$room_version"

    // optional - Guava support for Room, including Optional and ListenableFuture
    implementation "androidx.room:room-guava:$room_version"

    // optional - Test helpers
    testImplementation "androidx.room:room-testing:$room_version"

    // optional - Paging 3 Integration
    implementation "androidx.room:room-paging:2.4.0-beta01"
}

### Primary components
- The database class that holds the database and serves as the main access point for the underlying connection to your app's persisted data.

- Data entities that represent tables in your app's database.
- Data access objects (DAOs) that provide methods that your app can use to query, update, insert, and delete data in the database.

![Room library architecture.](https://developer.android.com/images/training/data-storage/room_architecture.png)


## Defining data using Room entities 

When you use the Room persistence library to store your app's data, you define entities to represent the objects that you want to store. Each entity corresponds to a table in the associated Room database, and each instance of an entity represents a row of data in the corresponding table.


### Anatomy of an entity

Define each Room entity as a class that is annotated with @Entity. A Room entity includes fields for each column in the corresponding table in the database, including one or more columns that comprise the primary key.

### Define a primary key

Each Room entity must define a primary key that uniquely identifies each row in the corresponding database table. 


### Define a composite primary key

If you need instances of an entity to be uniquely identified by a combination of multiple columns, you can define a composite primary key by listing those columns in the primaryKeys property of @Entity.

### Ignore fields

By default, Room creates a column for each field that's defined in the entity. If an entity has fields that you don't want to persist, you can annotate them using @Ignore


## Define relationships between objects 

### Two possible approaches

In Room, there are two ways to define and query a relationship between entities: you can model the relationship using either an intermediate data class with embedded objects, or a relational query method with a multimap return type.

### Intermediate data class

In the intermediate data class approach, you define a data class that models the relationship between your Room entities. This data class holds the pairings between instances of one entity and instances of another entity as embedded objects.


## Accessing data using Room DAOs

When you use the Room persistence library to store your app's data, you interact with the stored data by defining data access objects, or DAOs. Each DAO includes methods that offer abstract access to your app's database.

### Anatomy of a DAO

There are two types of DAO methods that define database interactions:

- Convenience methods that let you insert, update, and delete rows in your database without writing any SQL code.
- Query methods that let you write your own SQL query to interact with the database.


### Convenience methods

Room provides convenience annotations for defining methods that perform simple inserts, updates, and deletes without requiring you to write a SQL statement.

1. **Insert** 

    The @Insert annotation allows you to define methods that insert their parameters into the appropriate table in the database.

2. **Update**

   The @Update annotation allows you to define methods that update specific rows in a database table. Similarly to @Insert methods, @Update methods accept data entity instances as parameters.

3. **Delete**

   The @Delete annotation allows you to define methods that delete specific rows from a database table. Similarly to @Insert methods, @Delete methods accept data entity instances as parameters.


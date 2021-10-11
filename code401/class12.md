# What I've Learned at the 12th lecture of 401 code...

## Working with Relationships in Spring Data REST

1. One-to-One Relationship

  - The Data Model
  - The Repositories
  - Creating the Resources
  - Creating the Associations

2. One-to-Many Relationship

   A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.


  - The Data Model

  - The Repository

  - The Association Resources

3. Many-to-Many Relationship

  - The Data Model

  - The Repository

  - The Association Resources


## Integration Testing in Spring

  Integration testing plays an important role in the application development cycle by verifying the end-to-end behavior of a system.


**Preparation**

1. Several Maven dependencies are required for running the integration tests we'll use in this article. First and foremost, we'll need the latest junit-jupiter-engine, junit-jupiter-api, and Spring test dependencies.

2. Spring MVC Test Configuration

  - Enable Spring in Tests with JUnit 5
  - JUnit 5 defines an extension interface through which classes can integrate with the JUnit test.
  - We can enable this extension by adding the @ExtendWith annotation to our test classes and specifying the   extension class to load. To run the Spring test, we use SpringExtension.class.


3. The WebApplicationContext Object : it provides a web application configuration. It loads all the application beans and controllers into the context.

4. Mocking Web Context Beans
  MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.

5. Verify Test Configuration
  Checking that a GreetController.java bean exists in the web context. This ensures that Spring beans are loaded properly. At this point, the setup of the integration test is done.



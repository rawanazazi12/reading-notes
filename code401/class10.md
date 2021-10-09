# What I've Learned at the 10th lecture of 401 code...

## Spring MVC and Thymeleaf

### Spring MVC and Thymeleaf: how to access data from templates

1. In a typical Spring MVC application, @Controller classes are responsible for preparing a model map with data and selecting a view to be rendered. 

2. This model map allows for the complete abstraction of the view technology and, in the case of Thymeleaf, it is transformed into a Thymeleaf context object (part of the Thymeleaf template execution context) that makes all the defined variables available to expressions executed in templates.


3. Spring model attributes
 Spring MVC calls the pieces of data that can be accessed during the execution of views model attributes. The equivalent term in Thymeleaf language is context variables.


4. There are several ways of adding model attributes to a view in Spring MVC:

  - Add attribute to Model via its addAttribute method

  - Return ModelAndView with model attributes included

  - Expose common attributes via methods annotated with @ModelAttribute:

5. Request parameters

   Request parameters can be easily accessed in Thymeleaf views. Request parameters are passed from the client to server like:

     `https://example.com/query?q=Thymeleaf+Is+Great!`

6. Session attributes               
  adding mySessionAttribute to session

7. ServletContext attributes                      
   The ServletContext attributes are shared between requests and sessions. In order to access ServletContext  
8. Spring beans      
  Thymeleaf allows accessing beans registered at the Spring Application Context with the @beanName syntax


9. @urlService refers to a Spring Bean registered at your context . 


## Serving Web Content with Spring MVC

#### Starting with Spring Initializr

To manually initialize the project:

1. Navigate to https://start.spring.io. This service pulls in all the dependencies you need for an application and does most of the setup for you.

2. Choose either Gradle or Maven and the language you want to use. This guide assumes that you chose Java.

3. Click Dependencies and select Spring Web, Thymeleaf, and Spring Boot DevTools.

4. Click Generate.

5. Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.
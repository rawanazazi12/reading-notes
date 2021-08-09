# What I've Learned at the 13th lecture of 301 code...

## Status Codes Based On REST Methods

1. What is a status code 202?                
   202 Accepted - Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future.

2. What is a status code 308?             
   308 Permanent Redirect - This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them. 

3. What code would you use if an update didn’t return data to a client?           
   204 No Content  
 
4. What is the ‘Forbidden’ status code?                 
   403 Forbidden - The client has authorized or doesn’t need to authorize itself, but still has no permissions to access the resource.  

5. What is middleware?           
   A middleware is basically a function that will the receive the Request and Response objects, just like your route Handlers do. 

6. What does `app.use(express.json()) do`?              
   express. json() is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app.

7. What does the /:id mean in a route?
   Defining the route path

8. What is the difference beween PUT and PATCH?

   - PUT: PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource.
   - PATCH method supplies a set of instructions to modify the resource.

9. How do you make a defalut value in a schema?
   Using mongoose.schema

10. What does a 500 error status code mean?
    Internal Server Error server error response.

11. What is the difference between a status 200 and a status 201?
    - 200:OK - It’s the basic status code to tell the client everything went good. Since we don’t create endpoint  accessible resource when creating an access token, we can use 200 as a status for that action.
    - 201 Created :The most fitting for Create operations. This code should signal backend-side resource creation and come along with a Location header that defines the most specific URL for that newly created resource.
   

## Things I want to know more about
   I want to learn more about status code, so I can understand the code much better.


### RESOURSES

  - [Status Codes Based On REST Methods](https://www.moesif.com/blog/technical/api-design/Which-HTTP-Status-Code-To-Use-For-Every-CRUD-App/)
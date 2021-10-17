# What I've Learned at the 15th lecture of 401 code...

## Spring Boot and OAuth2

1. How to build a sample app doing various things with "social login" using OAuth 2.0 and Spring Boot.

single-provider single-sign on, and works up to a client with a choice of authentication providers: GitHub or Google.

2. The samples are all single-page apps using Spring Boot and Spring Security on the back end. They also all use plain jQuery on the front end.

3. All samples are implemented using the native OAuth 2.0 support in Spring Boot.

4. There are several samples building on each other, adding new features at each step:

  - simple: a very basic static app with just a home page and unconditional login via Spring Boot’s OAuth 2.0 configuration properties (if you visit the home page, you will be automatically redirected to GitHub).

  - click: adds an explicit link that the user has to click to login.

  - logout: adds a logout link as well for authenticated users.

  - two-providers: adds a second login provider so the user can choose on the home page which one to use.

  - custom-error: adds an error message for unauthenticated users, and a custom authentication based on GitHub’s API


5. Each app can be imported into an IDE. You can run the main method in SocialApplication to start an app. 


## Single Sign On With GitHub

1. Creating a New Project
    - First, you need to create a Spring Boot application, which can be done in a number of ways. The easiest is to go to https://start.spring.io and generate an empty project (choosing the "Web" dependency as a starting point). 


    - You can then import that project into your favorite IDE (it’s a normal Maven Java project by default), or just work with the files and mvn on the command line.


2. In your new project, create index.html in the src/main/resources/static folder.


## Securing the Application with GitHub and Spring Security

To make the application secure, you can simply add Spring Security as a dependency. Since you’re wanting to do a "social" login (delegate to GitHub), you should include the Spring Security OAuth 2.0 Client starter.


## Add a New GitHub App

- To use GitHub’s OAuth 2.0 authentication system for login, you must first Add a new GitHub app.

- Select "New OAuth App" and then the "Register a new OAuth application" page is presented. Enter an app name and description. Then, enter your app’s home page, which should be http://localhost:8080, in this case. Finally, indicate the Authorization callback URL as http://localhost:8080/login/oauth2/code/github and click Register Application.

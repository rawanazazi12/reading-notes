# What I've Learned at the 14th lecture of 401 code...

## Spring Security Architecture

### Authentication and Access Control

1. Application security boils down to two more or less independent problems:

  - authentication (who are you?)
  - authorization (what are you allowed to do?)

2. Authentication : The main strategy interface for authentication is AuthenticationManager

  - An AuthenticationManager can do one of 3 things in its authenticate() method:
    1. Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.
    2. Throw an AuthenticationException if it believes that the input represents an invalid principal.
    3. Return null if it cannot decide.

3. AuthenticationException is a runtime exception. It is usually handled by an application in a generic way, depending on the style or purpose of the application.

4. The most commonly used implementation of AuthenticationManager is ProviderManager, which delegates to a chain of AuthenticationProvider instances.

5. AuthenticationManager hierarchy using ProviderManager

![AuthenticationManager](https://github.com/spring-guides/top-spring-security-architecture/raw/main/images/authentication.png)


### Customizing Authentication Managers

1. Spring Security provides some configuration helpers to quickly get common authentication manager features set up in your application. 

2. The most commonly used helper is the AuthenticationManagerBuilder, which is great for setting up in-memory, JDBC, or LDAP user details or for adding a custom UserDetailsService.

### Authorization or Access Control

1. Once authentication is successful, we can move on to authorization, and the core strategy here is AccessDecisionManager.

2. There are three implementations provided by the framework and all three delegate to a chain of AccessDecisionVoter instances, a bit like the ProviderManager delegates to AuthenticationProviders.

3. An AccessDecisionVoter considers an Authentication (representing a principal) and a secure Object


### Web Security

1. Spring Security in the web tier (for UIs and HTTP back ends) is based on Servlet Filters, so it is helpful to first look at the role of Filters generally.

2. The following picture shows the typical layering of the handlers for a single HTTP request.
![HTTP request](https://github.com/spring-guides/top-spring-security-architecture/raw/main/images/filters.png)



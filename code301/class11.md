# What I've Learned at the 11th lecture of 301 code...

## OAuth

1. What is OAuth?             
   OAuth allows websites and services to share assets among users. It is widely accepted, but be aware of its vulnerabilities.

2. Give an example of what using OAuth would look like:                   
   The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon.

3. How does OAuth work? What are the steps that it takes to authenticate the user?

    1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
    2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
    3. The first site gives this token and secret to the initiating user’s client software.
    4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
    5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
    6. The user approves (or their software silently approves) a particular transaction type at the first website.
    7. The user is given an approved access token (notice it’s no longer a request token).
    8. The user gives the approved access token to the first website.
    9. The first website gives the access token to the second website as proof of authentication on behalf of the user.
    10. The second website lets the first website access their site on behalf of the user.
    11. The user sees a successfully completed transaction occurring.
    12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. 

  
4. What is OpenID?                            
   OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans.

## Authorization and Authentication flows

1. What is the difference between authorization and authentication?          
    **Authentication** is the process of verifying who a user is.
     **Authentication** is the process of verifying who a user is.

2. What is Authorization Code Flow?                
   The authorization code grant type is used to obtain both access
   tokens and refresh tokens and is optimized for confidential clients.

3. What is Implicit Flow with Form Post?        
   As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets.

4. What is Client Credentials Flow?                          
   The client can request an access token using only its client credentials (or other supported means authentication) when the client is requesting access to the protected resources under its
   control.

5. What is Device Authorization Flow?              
   The OAuth 2.0 device authorization grant is designed for Internet connected devices that either lack a browser to perform a user-agent based authorization.

6. What is Resource Owner Password Flow?
   This grant type is suitable for clients capable of obtaining the resource owner's credentials (username and password, typically using an interactive form).


## Things I want to know more about:

   I want to learn more about Outh usage and how to deal with it.



### RESOURSES

  - [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html) 

  - [Authorization and Authentication flows](https://auth0.com/docs/flows)




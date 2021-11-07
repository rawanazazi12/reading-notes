# Read: 32 - Serverless and Amplify

- Serverless applications are event-driven cloud-based systems where application development rely solely on a combination of third-party services, client-side logic and cloud-hosted remote procedure calls (Functions as a Service).

- Here are some of the currently available cloud services:

   - AWS Lambda
   - Google Cloud Functions
   - Azure Functions
   - IBM OpenWhisk
   - Alibaba Function Compute
   - Iron Functions
   - Auth0 Webtask
   - Oracle Fn Project
   - Kubeless
   

- Traditional vs. Serverless Architecture

![Traditional vs. Serverless Architecture](https://hackernoon.com/hn-images/1*x_v5NRC3TTMt1MaYl1gMUg.jpeg)

### Functions as a Service (FaaS)

  FaaS is an implementation of Serverless architectures where engineers can deploy an individual function or a piece of business logic.

  
### Principles of FaaS:

- Complete management of servers
- Invocation based billing
- Event-driven and instantaneously scalable

### Key properties of FaaS:

Independent, server-side, logical functions

FaaS are similar to the functions you’re used to writing in programming languages, small, separate, units of logic that take input arguments, operate on the input and return the result.


### The Serverless App

A Serverless solution consists of a web server, Lambda functions (FaaS), security token service (STS), user authentication and database.

- Client Application — The UI of your application is rendered client side in Modern Frontend Javascript App which allows us to use a simple, static web server.
- Web Server — Amazon S3 provides a robust and simple web server. All of the static HTML, CSS and JS files for our application can be served from S3.
- Lambda functions (FaaS) — They are the key enablers in Serverless architecture. 

- Security Token Service (STS) — generates temporary AWS credentials (API key and secret key) for users of the application.

- User Authentication — AWS Cognito is an identity service which is integrated with AWS Lambda. 

- Database — AWS DynamoDB provides a fully managed NoSQL database.


### Benefits of Serverless Architecture

**From business perspective**

1. The cost incurred by a serverless application is based on the number of function executions, measured in milliseconds instead of hours.
2. Process agility: Smaller deployable units result in faster delivery of features to the market, increasing the ability to adapt to change.
3. Cost of hiring backend infrastructure engineers goes down.
4. Reduced operational costs


**From developer perspective**

1. Reduced liability, no backend infrastructure to be responsible for.
2. Zero system administration.
3. Easier operational management.
4. Fosters adoption of Nanoservices, Microservices, SOA Principles.
5. Faster set up.


**From user perspective**

1. If businesses are using that competitive edge to ship features faster, then customers are receiving new features quicker than before.
2. It is possible that users can more easily provide their own storage backend(i.e Dropbox, Google Drive).
3. It’s more likely that these kinds of apps may offer client-side caching, which provides a better offline experience.
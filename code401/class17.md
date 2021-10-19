# What I've Learned at the 17th lecture of 401 code...

## Using WebSocket to build an interactive web application

1. WebSocket is a thin, lightweight layer above TCP. This makes it suitable for using “subprotocols” to embed messages.

2. You will build a server that accepts a message that carries a user’s name. In response, the server will push a greeting into a queue to which the client is subscribed.

3. What will be needed:
  - A favorite text editor or IDE
  - JDK 1.8 or later
  - Gradle 4+ or Maven 3.2+
  - Spring Tool Suite (STS)
  - IntelliJ IDEA


4. Starting with Spring Initializr
   To manually initialize the project:

   1. Navigate to https://start.spring.io. This service pulls in all the dependencies you need for an application and does most of the setup for you.

   2. Choose either Gradle or Maven and the language you want to use. This guide assumes that you chose Java.

   3. Click Dependencies and select Websocket.

   4. Click Generate.

   5. Download the resulting ZIP file, which is an archive of a web application that is configured with your choices.


5. If your IDE has the Spring Initializr integration, you can complete this process from your IDE.

6. Adding Dependencies
  The Spring Initializr does not provide everything you need in this case. For Maven, you need to add the following dependencies:

    >dependencies {
	implementation 'org.springframework.boot:spring-boot-starter-websocket'                    
	implementation 'org.webjars:webjars-locator-core'                                     
	implementation 'org.webjars:sockjs-client:1.0.2'                              
	implementation 'org.webjars:stomp-websocket:2.3.3'                            
	implementation 'org.webjars:bootstrap:3.3.7'                            
	implementation 'org.webjars:jquery:3.1.1-1'                                        
	testImplementation 'org.springframework.boot:spring-boot-starter-test'
   }
   >

7. Create a Resource Representation Class
  Begin the process by thinking about service interactions.

8. Create a Message-handling Controller
   In Spring’s approach to working with STOMP messaging, STOMP messages can be routed to @Controller classes. For example, the GreetingController (from src/main/java/com/example/messagingstompwebsocket/GreetingController.java) is mapped to handle messages to the /hello destination.

 
9. Configure Spring for STOMP messaging                        
   Create a Java class named WebSocketConfig that resembles the following listing (from src/main/java/com/example/messagingstompwebsocket/WebSocketConfig.java
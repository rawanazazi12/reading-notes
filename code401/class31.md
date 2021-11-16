# Read: 39 - Kinesis

## ANALYTICS

The Analytics category enables you to collect analytics data for your App. The Analytics category comes with built-in support for Amazon Pinpoint and Amazon Kinesis (Kinesis support is currently only available in the Amplify JavaScript library).


## Set up Analytics backend

Run the following command in your project's root folder. The CLI will prompt configuration options for the Analytics category such as Amazon Pinpoint resource name and analytics event settings.

`amplify add analytics`

? Select an Analytics provider (Use arrow keys)                                  
    `Amazon Pinpoint`                                        
? Provide your pinpoint resource name:                                    
    `yourPinpointResourceName`                                                                                    
? Apps need authorization to send analytics events. Do you want to allow guests and unauthenticated users to send     
analytics events? (we recommend you allow this when getting started)                                              
    `Yes`

- To deploy your backend, run:

`amplify push`


## Install Amplify Libraries

Expand Gradle Scripts, open build.gradle (Module: app). You will already have configured Amplify by following the steps in the Project Setup walkthrough.

Add Analytics by adding these libraries into the dependencies block:

dependencies {                                               
    // Add these lines in `dependencies`                                               
    implementation 'com.amplifyframework:aws-analytics-pinpoint:1.29.0'                                          
    implementation 'com.amplifyframework:aws-auth-cognito:1.29.0'                                           
}



## Initialize Amplify Analytics

To initialize the Amplify Auth and Analytics categories you call Amplify.addPlugin() method for each category. To complete initialization call Amplify.configure().

- Add the following code to your onCreate() method in your application class:

`Amplify.addPlugin(new AWSCognitoAuthPlugin());`                                                               
`Amplify.addPlugin(new AWSPinpointAnalyticsPlugin(this));`





## Record events
To record an event, create an AnalyticsEvent and call Amplify.Analytics.recordEvent() to send it:

AnalyticsEvent event = AnalyticsEvent.builder()                                                      
    .name("PasswordReset")                          
    .addProperty("Channel", "SMS")                               
    .addProperty("Successful", true)                       
    .addProperty("ProcessDuration", 792)                                     
    .addProperty("UserAge", 120.3)                       
    .build();                                         

Amplify.Analytics.recordEvent(event);


## View Analytics console

From the terminal run the following command.

`amplify console analytics`
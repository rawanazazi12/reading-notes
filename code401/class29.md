# Read: 37 - S3
## Introduction to Amazon S3

- What is Amazon S3?

   Amazon Simple Storage Service (Amazon S3) is an object storage service that offers industry-leading scalability, data availability, security, and performance.

- Storage classes      

  Amazon S3 offers a range of storage classes designed for different use cases. 
  You can store data with changing or unknown access patterns in S3 Intelligent-Tiering, which optimizes storage costs by automatically moving your data between four access tiers when your access patterns change. 

- Storage management

  Amazon S3 has storage management features that you can use to manage costs, meet regulatory requirements, reduce latency, and save multiple distinct copies of your data for compliance requirements.

- Data processing              

  To transform data and trigger workflows to automate a variety of other processing activities at scale, you can use the following features.

  - S3 Object Lambda : Add your own code to S3 GET requests to modify and process data as it is returned to an application. 
      
  - Event notifications : Trigger workflows that use Amazon Simple Notification Service (Amazon SNS), Amazon Simple Queue Service (Amazon SQS), and AWS Lambda when a change is made to your S3 resources.


### How Amazon S3 works

Amazon S3 is an object storage service that stores data as objects within buckets. An object is a file and any metadata that describes the file. A bucket is a container for objects.


## S3 with Amplify

- ### STORAGE                  
  The Amplify Storage category provides an interface for managing user content for your app in public, protected, or private storage buckets. 

  
**Prerequisites**                                     
An Android application targeting Android API level 16 (Android 4.1) or above.

- To start provisioning storage resources in the backend, go to your project directory and execute the command:

`amplify add storage`

- To push your changes to the cloud, execute the command:

`amplify push`

Upon completion, amplifyconfiguration.json will be updated to reference a newly provisioned S3 bucket.


### Install Amplify Libraries

- Expand Gradle Scripts, open build.gradle (Module: app).
- Add these libraries into the dependencies block:

  dependencies {
    `implementation 'com.amplifyframework:aws-storage-s3:1.28.3'`                             
    `implementation 'com.amplifyframework:aws-auth-cognito:1.28.3'  `                                    
  }


### Initialize Amplify Storage

- To initialize the Amplify Auth and Storage categories you call Amplify.addPlugin() method for each category. To complete initialization call Amplify.configure().

- Add the following code to your onCreate() method in your application class:
 
  `Amplify.addPlugin(new AWSCognitoAuthPlugin());`                                           
  `Amplify.addPlugin(new AWSS3StoragePlugin());`


###  Uploading data to your bucket

  To upload to S3 from a data object, specify the key and the data object to be uploaded.

       private void uploadFile() {
       File exampleFile = new File(getApplicationContext().getFilesDir(), "ExampleKey");

      try {
        BufferedWriter writer = new BufferedWriter(new FileWriter(exampleFile));
        writer.append("Example file contents");
        writer.close();
      } catch (Exception exception) {
        Log.e("MyAmplifyApp", "Upload failed", exception);
      }

       Amplify.Storage.uploadFile(
            "ExampleKey",
            exampleFile,
            result -> Log.i("MyAmplifyApp", "Successfully uploaded: " + result.getKey()),
            storageFailure -> Log.e("MyAmplifyApp", "Upload failed", storageFailure)
      );
   }

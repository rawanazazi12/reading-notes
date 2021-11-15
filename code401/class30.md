# Amazon SNS

- Amazon Simple Notification Service (Amazon SNS) is a fully managed messaging service for both  application-to-application (A2A) and application-to-person (A2P) communication.


## Benefits

- Modernize and decouple your applications

  Amazon SNS enables you to modernize your applications and decouple them into smaller, independent components that are easier to develop, deploy, and maintain.

- Send messages directly to millions of users

  Amazon SNS enables you to send messages or notifications directly to users with SMS text messages to over 200 countries, mobile push on Apple, Android, and other platforms or email (SMTP).

- Automatically scale your workload

  Amazon SNS leverages the proven AWS cloud to dynamically scale with your application. Amazon SNS is a fully managed service, taking care of the heavy lifting related to capacity planning, provisioning, monitoring, and patching.

- Ensure accuracy with message ordering and deduplication

  Amazon SNS FIFO topics work with Amazon SQS FIFO queues to ensure messages are delivered in a strictly ordered manner and are only processed once (deduplicated)

- Simplify your architecture with Message Filtering

  Amazon SNS helps you simplify your pub/sub messaging architecture by offloading the message filtering logic from your subscriber systems, and message routing logic from your publisher systems.


## Getting started with Amazon SNS

- Step 1: Create a topic

  1. Sign in to the Amazon SNS console.

  2. In the left navigation pane, choose Topics.

  3. On the Topics page, choose Create topic.

  4. By default, the console creates a FIFO topic. Choose Standard.

  5. In the Details section, enter a Name for the topic, such as MyTopic.

  6. Scroll to the end of the form and choose Create topic.


- Step 2: Create a subscription to the topic

  1. In the left navigation pane, choose Subscriptions.

  2. On the Subscriptions page, choose Create subscription.

  3. On the Create subscription page, choose the Topic ARN field to see a list of the topics in your AWS account.

  4. Choose the topic that you created in the previous step.

  5. For Protocol, choose Email.

  6. For Endpoint, enter an email address that can receive notifications.

  7. Choose Create subscription.

  8. The console opens the new subscription's Details page.


- Step 3: Publish a message to the topic

  1. In the left navigation pane, choose Topics.

  2. On the Topics page, choose the topic that you created earlier, and then choose Publish message.

  3. The console opens the Publish message to topic page.

  4. (Optional) In the Message details section, enter a Subject, such as:

      Hello from Amazon SNS!

  5. In the Message body section, choose Identical payload for all delivery protocols, and then enter a message body, such as:

     Publishing a message to an SNS topic.

  7. Choose Publish message.

     The message is published to the topic, and the console opens the topic's Details page.

  8. Check your email inbox and verify that you received an email from Amazon SNS with the published message.


- Step 4: Delete the subscription and topic
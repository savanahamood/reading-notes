# AWS: Events

### AWS SQS vs SNS

**1. What is the difference betweeen SQS and SNS?**

SQS is primarily used for queuing and asynchronous communication, while SNS is used for real-time, push-based messaging to multiple subscribers. Depending on your application's needs, you might choose one or both services to achieve the desired decoupling and scalability.


**2. What are some use cases for both SNS and SQS?**

* Send notifications about events and updates to multiple recipients.
* Deliver push notifications to mobile app users across various platforms.
* Distribute messages to multiple microservices, applications, or instances in a fan-out pattern.


### AWS SNS and SQS

**1. Describe how to use SQS and SNS in a “fanout” pattern.**

Here's how to use SQS and SNS in a fanout pattern:

* Create an SNS Topic:
First, you need to create an SNS topic. Go to the AWS Management Console, navigate to the SNS service, and click on "Create topic."
Give your topic a descriptive name and optional display name, then click "Create topic."
* Subscribe SQS Queues to the SNS Topic:
After creating the SNS topic, you need to subscribe one or more SQS queues to it. SQS queues act as subscribers in the fanout pattern.
Go to the SNS topic you just created, click on "Create subscription," and select "SQS" as the protocol.
Choose the SQS queue you want to subscribe to the topic and click "Create subscription." Repeat this step if you have multiple SQS queues.
* Publish Messages to the SNS Topic:
Now that you have SQS queues subscribed to the SNS topic, you can start publishing messages to the topic.
Go to the SNS topic's details page and click on "Publish message."
Write the message you want to send and click "Publish." The message will be sent to all the subscribed SQS queues.
* Processing Messages in SQS Queues:
Each subscribed SQS queue will receive a copy of the published message independently. This allows parallel processing of the message by different components or systems.
Your application or backend systems can process the messages in the SQS queues as needed. Each queue acts as an independent consumer.


**2. Explain how “push notifications” work, using SNS.**

Here's how push notifications work using SNS:

* Create an SNS Platform Application:
To send push notifications to specific platforms (e.g., iOS, Android, Web), you need to create an SNS platform application for each platform. Go to the AWS Management Console, navigate to SNS, and click on "Create platform application."
Select the platform for which you want to create the application (e.g., Apple Push Notification service - APNs for iOS or Firebase Cloud Messaging - FCM for Android), and follow the setup instructions to configure the application.
* Get Device Tokens or Registration IDs:
For each user's device or application that you want to send push notifications to, you need to obtain a unique device token (for iOS) or registration ID (for Android) from the respective platform's push notification service.
These tokens/IDs uniquely identify the device or application and act as the destination for push notifications.
* Subscribe Devices to the SNS Platform Application:
Once you have the device tokens or registration IDs, you need to subscribe them to the appropriate SNS platform application. This tells SNS which devices or applications should receive push notifications from the application.
Go to the SNS platform application you created earlier, click on "Create platform endpoint," and provide the device token or registration ID for the specific device or application you want to subscribe.
* Sending Push Notifications:
To send a push notification, you publish a message to the SNS platform application with the content of the notification and any other relevant data.
Go to the SNS platform application, click on "Publish a message," and specify the message payload, such as the notification title, body, and custom data.
SNS will then deliver the message to all the subscribed devices/applications using the respective push notification services (e.g., APNs for iOS or FCM for Android).
* Receiving Push Notifications:
The push notification service on each platform (e.g., APNs or FCM) will deliver the notification to the target devices or applications based on the device tokens/registration IDs.
The devices' operating systems handle the display of the push notification to the users based on their notification settings.

### SQS and SNS Basics

**1. How might a large scale, distributed application make use of a Queue system like SQS?**

By leveraging SQS, a large-scale, distributed application can achieve better scalability, fault tolerance, and performance. It provides an efficient way to manage communication between different components and services, enabling seamless handling of large workloads and enhancing the overall reliability of the application.




### Resources:
 [AWS SQS vs SNS](https://medium.com/awesome-cloud/aws-difference-between-sqs-and-sns-61a397bf76c5)

[AWS SNS and SQS](https://www.youtube.com/watch?v=mXk0MNjlO7A)

[SQS and SNS Basics](https://www.youtube.com/watch?v=UesxWuZMZqI)

[SNS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SNS.html)

[SQS Javascript SDK](https://docs.aws.amazon.com/AWSJavaScriptSDK/latest/AWS/SQS.html)
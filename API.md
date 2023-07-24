# AWS: API, Dynamo and Lambda

### AWS API Gateway Overview

**1. What is Amazon API Gateway?**

Amazon API Gateway is a fully managed service provided by Amazon Web Services (AWS) that allows developers to create, publish, maintain, monitor, and secure APIs (Application Programming Interfaces) at any scale. An API Gateway acts as a front-door for applications to access backend services and resources securely and efficiently.


**2. Why is Amazon API Gateway an important part of the Serverless ecosystem?**

API Gateway complements the serverless architecture by enabling developers to build serverless APIs without worrying about server provisioning, scaling, or infrastructure management. It seamlessly integrates with AWS Lambda, which allows you to implement the business logic of your APIs in stateless functions, known as Lambda functions.


**2.How does API Gateway integrate with other AWS services?**

Amazon API Gateway plays a crucial role in the serverless ecosystem by providing a secure, scalable, and easily manageable front-end for serverless applications, allowing developers to focus on building and deploying APIs without managing the underlying infrastructure.



### AWS API Gateway

**1.What are the some benefits of using Amazon API Gateway?**

* allowing your APIs to handle large numbers of concurrent requests without manual intervention.

* integrates with AWS Lambda, enabling you to build serverless applications where the business logic is implemented in stateless functions. This serverless architecture eliminates the need to manage servers, reducing operational overhead.

* API Gateway provides various security features such as access control, authentication, and authorization.

* it offers built-in logging and monitoring capabilities.


**2.What two API types might you choose from?**

* RESTful APIs (Representational State Transfer)
* WebSocket APIs


### AWS DynamoDB Guide

**1.What is DynamoDB?**

Amazon DynamoDB is a fully managed NoSQL database service provided by Amazon Web Services (AWS). It is designed to provide fast and predictable performance with seamless scalability, making it well-suited for a wide range of applications, from small-scale projects to large enterprise systems.


**2.Under what circumstances would you recommend DynamoDB over MongoDB?**

* For applications that demand very low read and write latencies and need to handle a high number of requests per second, DynamoDB's design for speed and performance makes it a strong candidat
* If you prefer a fully managed database service that takes care of most administrative tasks, such as backup, restore, scaling, and maintenance, DynamoDB's serverless nature
* If you are building your application in the AWS ecosystem and want tight integration with other AWS services, DynamoDB is a natural fit as it is an integral part of AWS.


### AWS DynamoDB

**1.Explain to a non-technical friend how DynamoDB works.**

DynamoDB is a powerful and magical digital notebook that stores and organizes your data, makes it super easy to find, and takes care of everything behind the scenes, so you can focus on what's important to you



### Dynamoose

**1.What is Dynamoose?**

Dynamoose is a JavaScript library and an Object-Data Mapping (ODM) library designed to work with Amazon DynamoDB, the fully managed NoSQL database service provided by AWS. Dynamoose simplifies the process of working with DynamoDB by allowing developers to interact with the database using familiar JavaScript syntax and object-oriented programming paradigms


**2.What are some key features of Dynamoose?**

* Object-Data Mapping (ODM)
* Schema Definition
* Model Creation
* CRUD Operations


### Resources:
 [AWS API Gateway Overview](https://www.serverless.com/amazon-api-gateway)

[AWS API Gateway](https://aws.amazon.com/api-gateway/)

[AWS DynamoDB Guide](https://www.dynamodbguide.com/what-is-dynamo-db/)

[AWS DynamoDB](https://aws.amazon.com/dynamodb/)

[Dynamoose](https://dynamoosejs.com/getting_started/Introduction)




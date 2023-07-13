# AWS: Cloud Servers
### AWS EC2
**1. What is an EC2 Instance?**
An EC2 (Elastic Compute Cloud) instance is a virtual server in the cloud provided by Amazon Web Services (AWS). It allows you to rent virtual machines with varying compute capacities and configurations, enabling you to run applications and services in a flexible and scalable manner.

**2. Name 2 use cases for EC2.** 
* Web Hosting: EC2 instances can be used to host websites, web applications, or blogs. You can choose an appropriate instance type based on your requirements and scale your infrastructure as needed.
* Batch Processing: EC2 instances can be used for batch processing tasks such as data analysis, rendering, or encoding. You can launch multiple instances to process large amounts of data in parallel.

**3. Provide 1 reason to use ECS instead of a service such as Heroku, Digital Ocean, or Render.com.**
ECS allows you to manage your own infrastructure and gives you more flexibility in terms of customization and scalability.


### EC2 For Humans
**1. Where can we find EC2 on the AWS Console?**
* Sign in to your AWS account.
* Open the AWS Management Console.
* In the search bar at the top, type "EC2" and select "EC2" from the suggestions.
* This will take you to the EC2 Dashboard where you can manage your EC2 instances, security groups, volumes, and other related resources.

**2. Explain the general difference between T2 Micro and XL.**
* T2 Micro:
Designed for general-purpose workloads.
Limited baseline CPU performance but can burst for short periods.
Smaller amount of memory and storage.
Suitable for lightweight workloads, development/testing environments, and low-traffic websites.
* XL:
Provides higher baseline CPU performance.
Offers larger compute capacity compared to T2 Micro.
More memory and storage capacity.
Suitable for resource-intensive applications, databases, high-traffic websites, and workloads requiring sustained CPU power.

**3. Explain a “Compute Cycle” to a non-technical friend.**
you can think of a compute cycle as a single step or operation that a computer takes to accomplish a task, just like you take steps to solve a problem. By performing many compute cycles, computers can carry out complex calculations, process data, and run various applications.


### Elastic Beanstalk
**1. What is Elastic Beanstalk?**
 Elastic Beanstalk is a fully managed service provided by AWS that simplifies the deployment and management of applications. It automates the process of setting up the underlying infrastructure, such as EC2 instances, load balancers, and databases, allowing developers to focus on writing code rather than worrying about infrastructure configuration.

**2. Describe the relationship between EC2 and Elastic Beanstalk.**
When you deploy an application using Elastic Beanstalk, it automatically provisions and manages the necessary EC2 instances and other AWS resources required to run your application.

**3. Name some benefits of using Elastic Beanstalk.**
* Easy Application Deployment.
* Auto Scaling: Elastic Beanstalk can automatically scale your application based on the configured settings.
* Monitoring and Health Management.
* Platform Support: Elastic Beanstalk supports multiple programming languages and platforms.


### Resources:
 [Virtual Machines](https://www.youtube.com/watch?v=yIVXjl4SwVo)

[VMS and the Cloud](https://www.youtube.com/watch?v=l0DfHUWMjsU)

[AWS EC2](https://aws.amazon.com/ec2/)

[EC2 For Humans](https://www.youtube.com/watch?v=lZMkgOMYYIg)

[Elastic Beanstalk](https://www.youtube.com/watch?v=SrwxAScdyT0)


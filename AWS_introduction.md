

# **AWS - Amazon Web Service**



Amazon Web Services (AWS) is one of the most widely used cloud platforms in the world. It offers a huge variety of tools and services that help businesses build, deploy, and scale applications easily. If you are just starting your cloud journey, it is important to get familiar with the most commonly used AWS services.







## Compute Services

AWS compute services provide virtualized and serverless environments for running applications, workloads, and containers in the cloud.



##### 1\. Amazon EC2 (Elastic Cloud Compute)

EC2 offers resizable compute capacity via virtual machines in the cloud.



Supports multiple instance types optimized for compute, memory, or storage.

Users can select AMIs (Amazon Machine Images) with desired OS.

Integration with Auto Scaling, Elastic Load Balancing, and EBS.

Use Case: Deploy a Linux EC2 instance to run a LAMP stack.



##### 2\. Amazon Lambda

Amazon Lambda is a serverless compute service that executes code in response to triggers/events.



Supports various runtimes (Node.js, Python, Java, Go, etc.).

Executes based on events (e.g., S3 upload, API Gateway, SNS).

Pay-per-use billing model (per request and execution time).

Use Case: Invoke a Python function to process data when uploaded to S3.



##### 3\. Amazon ECS / EKS

Managed services for orchestrating containers in AWS.



ECS: Native container orchestration for Docker containers, integrated with AWS tools.

EKS: Managed Kubernetes environment, compatible with Kubernetes-native tooling.

Use Case: Deploy containerized microservices architecture.



##### 4\. AWS Fargate

Serverless compute engine for containers on ECS or EKS.



Eliminates need for provisioning and managing EC2 instances.

Automatically scales container workloads.

Use Case: Run stateless APIs in Docker containers using ECS + Fargate.



##### 5\. Amazon Elastic Beanstalk

Amazon Elastic Beanstalk is a service from AWS that helps you easily deploy and manage web applications. You just upload your code, and the deployment part is handled by Elastic Beanstalk (from capacity provisioning, load balancing, and auto-scaling to application health monitoring).



Supports Java, Python, Node.js, .NET, PHP, Ruby, Go, and Docker.

Handles provisioning, load balancing, autoscaling, and monitoring.

Use Case: Deploy a Django application via ZIP upload.







## Database Services

##### 6\. Amazon RDS (Relational Database Services) 

Amazon RDS is a managed database service from AWS that supports databases like PostgreSQL, MariaDB, MySQL. With RDS, you can easily create, run, and scale databases in the cloud without managing hardware or installing software.



Supports automated backups, replication, Multi-AZ, and read replicas.

Monitoring via CloudWatch and performance insights.

Use Case: Deploy a Multi-AZ PostgreSQL backend for a SaaS platform.



##### 7\. Dynamo DB

DynamoDB is a serverless NoSQL database from AWS that stores data as key-value pairs and documents. It is made to handle very large, high-speed applications. DynamoDB can process up to 10 trillion requests per day and handle over 20 million requests every second.



Supports DAX (in-memory caching), on-demand or provisioned throughput, and streams.

Fully serverless with auto-scaling and encryption.

Use Case: Real-time leaderboard in a multiplayer gaming app.



##### 8\. Amazon Aurora

High-performance, MySQL and PostgreSQL-compatible relational database.



Distributed, fault-tolerant, and self-healing storage.

Auto-scaling, Global Databases, and up to 15 read replicas.

Use Case: Backend database for high-traffic e-commerce platform.



Storage Services 

AWS storage services provide scalable, durable, and secure storage options for object, block, and file data.



##### 9\. Amazon S3 (Simple Storage Service)

Amazon S3 is a popular AWS service that makes it easy to store and access data from anywhere at any time. It is a type of object storage that offers high performance, strong security, and can grow as your data grows.



Supports versioning, lifecycle policies, and cross-region replication.

Provides high durability (99.999999999%).

Use Case: Store static website assets or data lake objects.



##### 10\. Amazon EBS (Elastic Block Store)

Amazon EBS is a storage service made for Amazon EC2. Provides persistent block storage volumes for EC2 instances.



Supports SSD (gp3, io2) and HDD (st1, sc1) volume types.

Volumes are encrypted and support point-in-time snapshots.

Use Case: Attach EBS to EC2 instance for MySQL database storage.



##### 11\. Amazon EFS (Elastic File System)

Amazon EFS (Elastic File System) is a simple and serverless system where you can create and configure file systems without provisioning, deploying, patching, and maintaining. It is a scalable NFS file system made for use in AWS cloud services and on-premises resources. Also, it has no minimum fee or setup charge. You pay for the storage you use such as - 



for provisioned throughput

automatically expand and shrink as per the addition and removal of files

read and write access to data stored in Infrequent Access storage classes

It is a scalable service where you can scale up to petabytes without thinking about the performance of the application. 



##### 12\. Amazon FSx

Managed file systems for high-performance and Windows-compatible workloads.



FSx for Windows File Server: Fully compatible with SMB and AD.

FSx for Lustre: High-throughput POSIX file system for HPC workloads.

Use Case: Shared file system for .NET apps in an AD environment.



Networking \& Content Delivery

Services for securely connecting AWS resources, delivering content globally, and managing network infrastructure.



##### 13\. Amazon VPC (Virtual Private Cloud)

Amazon VPC is a service that lets you create your own private area inside the AWS cloud. In this private space, you can set up and manage AWS resources safely and on a large scale.



Custom IP ranges, subnets, route tables, NAT gateways, and internet gateways.

Supports security groups, NACLs, and VPC peering.

Use Case: Deploy a secure, multi-tier web application.



##### 14\. Amazon CloudFront

Amazon Cloudfront is a Content Delivery Network (CDN) to distribute content with low latency.



Uses edge locations worldwide.

Integrates with S3, ELB, and Lambda@Edge.

Use Case: Cache static and dynamic website content globally.



##### 15\. Amazon Route 53

Amazon Route 53 is a highly available and scalable DNS and domain registration service.



Supports routing policies: latency-based, failover, geolocation, and weighted.

Offers DNS health checks and private hosted zones.

Use Case: Map a domain to an S3 static website with latency-based routing.



##### 16\. Elastic Load Balancer (ELB)

Elastic Load Balancer (ELB) is an AWS service that helps distribute incoming network traffic across multiple servers. This ensures that no single server is overwhelmed with too much traffic and that users get fast and reliable responses.



ELB helps with high availability, fault tolerance, and the efficient management of traffic in a scalable way. It integrates well with services like EC2, ECS, and Lambda to manage large traffic loads and maintain a seamless user experience.

ELB fits into cloud environments that require automatic scaling, distributed traffic, and fault tolerance to keep services always available.

Supports SSL termination, sticky sessions, and path-based routing.

Use Case: Load balance HTTPS traffic across EC2 backend servers.



Types of Elastic Load Balancers:



There are three types of Elastic load balancers in AWS:



Application Load Balancer: Best for HTTP and HTTPS traffic (Layer 7 - Application Layer)

Network Load Balancer: Best for High-performance TCP/UDP traffic (Layer 4 - Transport Layer)

Gateway Load Balancer: Best for deploying, scaling, and managing third-party virtual appliances (e.g., firewalls, intrusion detection systems)

Security \& Identity Services

Services to manage user authentication, enforce least-privilege access, and protect resources.



##### 17\. Amazon IAM (Identity and Access Management)

Amazon IAM helps you control who can access and use AWS resources safely. It lets you decide who can sign in and what they are allowed to do.



Define users, groups, roles, and attach policies (JSON).

Supports MFA, permission boundaries, and service-linked roles.

Use Case: Assign EC2-only access to a developer group.



##### 18\. AWS WAF \& AWS Shield

Protects applications from web-based and DDoS attacks.



AWS WAF: Custom rules to block SQLi, XSS, and bad bots.

AWS Shield: DDoS protection (Standard and Advanced tiers).

Use Case: Secure a public API endpoint from layer 7 attacks.



Monitoring \& Analytics

Monitoring and analytics in AWS help you track the health, performance, usage, and security of your cloud infrastructure and applications. AWS offers built-in tools that give you real-time insights and help you take automated actions when something goes wrong.



##### 19\. Amazon Cloudwatch

Amazon Cloudwatch is a monitoring service for AWS resources and custom applications



Collects metrics like CPU usage, memory, disk I/O, request count, latency, etc.

Creates dashboards, alarms, and automated responses (e.g., auto-scaling or notifications).

Use Cases:



Monitor EC2, RDS, Lambda, ELB, etc.

Set alerts for high CPU or failed health checks.



##### 20\. AWS CloudTrail

A logging service that records all API calls and user activity in your AWS account.



Tracks who did what, when, and from where.

Stores logs in S3 and integrates with CloudWatch for analysis.

Use Case: Security audits, compliance, and forensic investigations.



##### 21\. AWS X-Ray

AWS X-Ray is a distributed tracing system to analyze and debug microservices-based applications.



Traces each user request through services like Lambda, ECS, API Gateway, etc.

Helps identify slow services, latency bottlenecks, and failures.

Use Case: Performance tuning and debugging for serverless or containerized apps.



##### 22\. AWS Config

AWS Config is a configuration management service.



Monitors and records the configuration history of AWS resources.

Evaluates compliance with desired settings (e.g., “EC2 must use encrypted EBS”).

Use cases:



Track changes to infrastructure

Ensure compliance and governance



##### 23\. Amazon QuickSight

Amazon QuickSight is a cloud-native business intelligence (BI) service.



Visualizes data from AWS services, S3, RDS, Redshift, and third-party sources.

Supports dashboards, reports, and predictive analytics using ML.

Use Cases:



Executive-level analytics and custom dashboards

Embedding data visualizations in apps



##### 24\. AWS Trusted Advisor

AWS Trusted Advisor is a recommendation engine for AWS best practices.



Scans your AWS environment for cost savings, performance, security, fault tolerance, and service limits.

Use cases:



Optimize resource usage and save money.

Improve account security posture.



##### 25\. AWS Cost Explorer

AWS Cost Explorer is a tool to analyze your AWS spending and usage trends.



Breaks down costs by service, resource, tag, and time range.

Forecasts future AWS bills based on usage.

Use cases:



Budget tracking and cost optimization

Chargeback and billing analysis

Machine Learning \& AI

AWS Machine Learning \& AI services provide powerful tools to build, train, and deploy intelligent applications. With pre-built models and customizable frameworks, developers can add capabilities like image recognition, natural language processing, and predictive analytics without deep ML expertise.



##### 26\. Amazon SageMaker

Amazon SageMaker is a machine learning service from AWS. It helps data scientists, business analysts, and developers easily build, train, and deploy machine learning models.

SageMaker makes data analysis faster and creates reports and predictions after processing the data. It can handle large amounts of both organized (structured) and unorganized (unstructured) data.

It also helps automate machine learning operations (MLOps), making the process more organized, easy to track, and transparent. This ensures proper control and clear records of all activities.

Messaging \& Notification Services

AWS Messaging \& Notification services enable reliable communication between applications and users. They support decoupling microservices, queuing messages, and sending real-time alerts via SMS, email, or push notifications all with high scalability and low latency.



##### 27\. Amazon SNS (Simple Notification Service)

Amazon SNS is a fully managed publish-subscribe (pub/sub) messaging service that enables systems, apps, and devices to send and receive notifications at scale. It supports two messaging types:



Application-to-Application (A2A): Communicates between microservices or applications.

Application-to-Person (A2P): Sends messages to users via SMS, email, or mobile push.

Use Case: An e-commerce platform uses SNS to send order confirmation emails to users and trigger internal workflows (e.g., notifying inventory services or shipping).



##### 28\. Amazon SQS (Simple Queue Service)

Amazon SQS is a message queuing service that decouples microservices, distributed systems, and serverless applications. It supports:



Standard Queues: Best-effort ordering with high throughput.

FIFO Queues: Guarantees exactly-once processing and first-in-first-out message order.

Use Case: A video processing system uploads videos to S3 and uses SQS to queue video conversion tasks. Worker nodes process jobs asynchronously, improving scalability and fault tolerance.



Business \& Productivity

AWS Business \& Productivity services help optimize operations, boost performance, and reduce costs. They automate scaling, improve app responsiveness, and streamline identity management for seamless user experiences.



##### 29\. Amazon Auto-Scaling

Amazon Auto Scaling dynamically adjusts the number of running compute resources (like EC2 instances) based on defined metrics or schedules. It supports:



Dynamic Scaling: Reacts to real-time load.

Predictive Scaling: Uses machine learning to forecast traffic and scale proactively.

Use Case: An online news portal experiences traffic spikes during major events. Auto Scaling ensures enough EC2 instances are available without manual intervention, minimizing costs during off-peak hours.



##### 30\. Amazon ElastiCache

Amazon ElastiCache provides fully managed in-memory caching using Redis or Memcached. It improves latency and throughput for applications that rely on frequently accessed data.



Use Case: A ride-hailing app uses ElastiCache to store real-time driver location data and session tokens, enabling quick access and a smoother user experience.



##### 31\. Amazon Cognito

Amazon Cognito manages user sign-up, sign-in, and access control for web and mobile applications. It supports federated identity (Google, Facebook, Apple, SAML) and native user pools with secure data synchronization.



Use Case: A fitness app allows users to log in using their Google or Facebook accounts, managed securely through Cognito. It also tracks user preferences and syncs workout history across devices.



Developer \& Serverless Services

AWS Developer \& Serverless services let you build and deploy applications quickly without managing servers. They simplify development, scale automatically, and reduce operational overhead.



##### 32\. Amazon LightSail

Amazon LightSail is a simplified VPS offering designed for developers, small businesses, and startups. It provides preconfigured compute, storage, and networking resources with a predictable monthly pricing model.



Use Case: A startup launches a simple WordPress blog using LightSail with one-click deployment, fixed costs, and optional scalability as the project grows. It avoids the complexity of setting up EC2, VPCs, and load balancers.




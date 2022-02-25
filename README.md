# Hello-world
 AWS file for GitHub


Within AWS, we commonly divide services into the “data plane” and the “control plane.” The data plane is responsible for delivering real-time service while control planes are used to configure the environment. For example, Amazon EC2 instances, Amazon RDS databases, and Amazon DynamoDB table read/write operations are all data plane operations. In contrast, launching new EC2 instances or RDS databases, or adding or changing table metadata in DynamoDB are all considered control plane operations. While high levels of availability are important for all of these capabilities, the data planes typically have higher availability design goals than the control planes. Therefore workloads with high availability requirements should avoid run-time dependency on control plane operations.



Cloud computing makes an abundance of monitoring and log information available for consumption, which can be used to define change-in-demand processes. The following is just a partial list of services and features that generate log and metric data.

* Amazon ECS, Amazon EC2, Elastic Load Balancing, AWS Auto Scaling, and Amazon EMR publish metrics for CPU, network I/O, and disk I/O averages. 
* Amazon CloudWatch Logs can be enabled for Amazon Simple Storage Service (Amazon S3), Classic Load Balancers, and Application Load Balancers. 
* VPC Flow Logs can be enabled to analyze network traffic into and out of a VPC. 
* AWS CloudTrail logs AWS account activity, including actions taken through the AWS Management Console, AWS SDKs, command line tools. 
* Amazon EventBridge delivers a real-time stream of system events that describes changes in AWS services. 
* AWS provides tooling to collect operating system-level logs and stream them into CloudWatch Logs. 
* Custom Amazon CloudWatch metrics can be used for metrics of any dimension. 
* Amazon ECS and AWS Lambda stream log data to CloudWatch Logs. 
* AWS AI and ML services, such as Amazon Rekognition, Amazon Lex, and Amazon Polly, provide metrics for successful and unsuccessful requests. 
* AWS IoT provides metrics for number of rule executions as well as specific success and failure metrics around the rules. 
* Amazon API Gateway provides metrics for number of requests, erroneous requests, and latency for your APIs. 
* AWS Personal Health Dashboard gives you a personalized view into the performance and availability of the AWS services underlying your AWS resources.
* Amazon CloudWatch Logs: You can store your logs in this service and inspect their contents. 
* Amazon CloudWatch Logs Insights: Is a fully managed service that enables you to run analyze massive logs in seconds. It gives you fast, interactive queries and visualizations.  
* AWS Config: You can see what AWS infrastructure was in use at different points in time. 
* AWS CloudTrail: You can see which AWS APIs were invoked at what time and by what principal. 


Security in the cloud: 

The amount of configuration work the customer must perform as part of their security responsibilities. For example, a service such as Amazon Elastic Compute Cloud (Amazon EC2) is categorized as Infrastructure as a Service (IaaS) and, as such, requires the customer to perform all of the necessary security configuration and management tasks. Customers that deploy an Amazon EC2 instance are responsible for management of the guest operating system (including updates and security patches), any application software or utilities installed by the customer on the instances, and the configuration of the AWS-provided firewall (called a security group) on each instance. For abstracted services, such as Amazon S3 and Amazon DynamoDB, AWS operates the infrastructure layer, the operating system, and platforms, and customers access the endpoints to store and retrieve data. Customers are responsible for managing their data (including encryption options), classifying their assets, and using IAM tools to apply the appropriate permissions.


Amazon Route 53, AWS Global Accelerator, Amazon CloudFront, Amazon API Gateway, and Elastic Load Balancing (ELB) all provide highly available public endpoints. You might also choose to evaluate AWS Marketplace software appliances for load balancing and proxying.


Amazon Route 53 is a scalable and highly available Domain Name System (DNS) service that connects user requests to infrastructure running in AWS-such as Amazon EC2 instances, Elastic Load Balancing load balancers, or Amazon S3 buckets–and can also be used to route users to infrastructure outside of AWS.

Amazon SQS queues and Elastic Load Balancers are just two ways to add an intermediate layer for loose coupling. Event-driven architectures can also be built in the AWS Cloud using Amazon EventBridge, which can abstract clients (event producers) from the services they rely on (event consumers). Amazon Simple Notification Service is an effective solution when you need high-throughput, push-based, many-to-many messaging. Using Amazon SNS topics, your publisher systems can fan out messages to a large number of subscriber endpoints for parallel processing.



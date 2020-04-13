* AWS TCO takes into consideration
- server 
- storage
- network
- IT Labour


* RDS supports automated backups, manual scaling and automated software updates


Question 3:
*  How can you ensure SQS messages are delivered in order?
FIFO queues are designed to ensure that the order in which messages are sent and received is strictly preserved and that each message is processed exactly once. See https://docs.aws.amazon.com/AWSSimpleQueueService/latest/SQSDeveloperGuide/FIFO-queues.html


* Dynamo db is a nosql database

> What is a CloudFormation stack?

A collection of aws resources that can be managed as a single unit.


A stack is a collection of AWS resources that you can manage as a single unit. In other words, you can create, update, or delete a collection of resources by creating, updating, or deleting stacks. All the resources in a stack are defined by the stack's AWS CloudFormation template.



* What is not a security best practice?

Don't use root access. MFA and IAM instead.



* You would like to decouple your application components from demand. What service would you use?
Amazon Simple Queue Service (Amazon SQS) offers a reliable, highly-scalable hosted queue for storing messages as they travel between applications or microservices. It moves data between distributed application components and helps you decouple these components.


You have an application that sends push messages to mobile devices. Which service should you use?
SNS
SNS can send push notifications See: https://docs.aws.amazon.com/sns/latest/dg/SNSMobilePush.html



Question 9:
Design for failure and nothing will fail, is a best practice?

Rule of thumb: Be a pessimist when designing architectures in the cloud; assume things will fail. In other words, always design, implement and deploy for automated recovery from failure. See: https://media.amazonwebservices.com/AWS_Cloud_Best_Practices.pdf


Amazon Redshift is a fully managed, petabyte-scale data warehouse service in the cloud. See: https://docs.aws.amazon.com/redshift/latest/mgmt/welcome.html


You would like to compare costs between AWS and onsite physical servers. What service is best to use?

aws tco

You would like to estimate the costs of a project on AWS. What service is best to use?

simple monthly calculator

You would like to investigate where costs are being wasted. What service is best to use?

AWS cost explorer

The only difference, other than price, between On-Demand instances and Spot Instances is that Spot instances can be interrupted by EC2 with two minutes of notification when the EC2 needs the capacity back.

True

An online resource to help you reduce cost, increase performance, and improve security by optimizing your AWS environment, _________ provides real time guidance to help you provision your resources following AWS best practices.

AWS trusted advisor

_________ is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. It automatically assesses applications for vulnerabilities or changes from best practices.

AWS Inspector 

Your users keep forgetting the account ID for logging in to the console. How can you help them?

create account alias

When you create IAM policies, follow the standard security advice of granting least privilege—that is, granting only the permissions required to perform a task. See: https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html#grant-least-privilege


Question 19:
A _________ tells Auto Scaling when and much to scale. You can create a _________  based on the occurrence of specified conditions (dynamic scaling) or you can create one based on a specific schedule.

A scaling plan tells Auto Scaling when and how to scale. For example, you can base a scaling plan on the occurrence of specified conditions (dynamic scaling) or on a schedule. An autoscaling policy defines how to scale and how much scaling to be applied. A scaling plan will reference a scaling policy.

*** 

Question 20:
What happens, by default, when one of the resources in a CloudFormation stack cannot be created?

By default, the “automatic rollback on error” feature is enabled. This will cause all AWS resources that AWS CloudFormation created successfully for a stack up to the point where an error occurred to be deleted. This is useful when, for example, you accidentally exceed your default limit of Elastic IP addresses, or you don’t have access to an EC2 AMI you’re trying to run. This feature enables you to rely on the fact that stacks are either fully created, or not at all, which simplifies system administration and layered solutions built on top of AWS CloudFormation.


Amazon CloudFront is a global content delivery network (CDN) service that securely delivers data, videos, applications, and APIs to your viewers with low latency and high transfer speeds from ________ around the World.
EDGE locations

What AWS service can you use to log API calls to SQS?

cloud trail (b/w aws services)



CloudWatch free monitoring for EC2 is at ________ intervals.

5minutes

You can use Amazon ________ to monitor, store, and access your log files from Amazon Elastic Compute Cloud (Amazon EC2) instances, AWS CloudTrail, Route 53, and other sources. You can then retrieve the associated log data from _________.
CWLogs

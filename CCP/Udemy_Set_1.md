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


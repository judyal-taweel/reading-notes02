## Amazon Simple Notification Service

Amazon Simple Notification Service (Amazon SNS) is a fully managed messaging service for both application-to-application (A2A) and application-to-person (A2P) communication.

The A2A pub/sub functionality provides topics for high-throughput, push-based, many-to-many messaging between distributed systems, microservices, and event-driven serverless applications. Using Amazon SNS topics, your publisher systems can fanout messages to a large number of subscriber systems including Amazon SQS queues, AWS Lambda functions and HTTPS endpoints, for parallel processing, and Amazon Kinesis Data Firehose. The A2P functionality enables you to send messages to users at scale via SMS, mobile push, and email.


### SNS with Amplify (and Firebase)

Amazon SNS is a managed messaging service that lets you decouple publishers from subscribers.
This is useful for system-to-system messaging for microservices, distributed architectures, and serverless applications
Amazon SNS lets you send push notifications to mobile apps, text messages to mobile phone numbers, and plain-text emails to email addresses.

### Steps to get started on Amazon SNS

Create a topic
Create a subscription to the topic
Publish a message to the topic
Delete the subscription and topic

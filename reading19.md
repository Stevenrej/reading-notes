# reading 19

## AWS SQS vs SNS

What is the difference betweeen SQS and SNS?

- SQS is a message queue service that helps decouple and scale microservices, distributed systems, and serverless applications. SNS is a messaging service that allows you to send messages to various endpoints, including SMS, email, and mobile push notifications, or invoke AWS Lambda functions.

What are some use cases for both SNS and SQS?

- Amazon Simple Queue Service (SQS) is a fully managed message queue service that enables you to decouple and scale microservices, distributed systems, and serverless applications. It helps you eliminate the complexity and overhead associated with managing and operating message-oriented middleware. Some use cases for SQS include decoupling microservices and distributed systems, building serverless applications, and integrating with other AWS services.

Amazon Simple Notification Service (SNS) is a fully managed messaging service that enables you to send messages to a large number of recipients or to other Amazon services. It allows you to send messages to various endpoints, including SMS texts, email addresses, and mobile device push notifications, or to invoke AWS Lambda functions to execute custom logic in response to messages. Some use cases for SNS include sending notifications, fanning out messages to multiple endpoints, and integrating with other AWS services.

## AWS SNS and SQS

Describe how to use SQS and SNS in a “fanout” pattern.

- To use SQS and SNS in a "fanout" pattern, you can use SNS to publish a message to a topic, and then have multiple SQS queues subscribed to that topic. When a message is published to the topic, it will be sent to all subscribed queues, allowing you to send the same message to multiple recipients or systems


Explain how “push notifications” work, using SNS.

- Create an SNS topic and register your mobile devices with the topic, using their device tokens.

When you want to send a push notification, publish a message to the SNS topic.

The message will be delivered to the subscribed mobile devices as a push notification.




## SQS and SNS Basics

How might a large scale, distributed application make use of a Queue system like SQS?

- Decoupling microservices and distributed systems: SQS can be used to decouple services by allowing them to communicate asynchronously via message queues. This enables each service to scale independently and improves fault tolerance.

Load balancing: SQS can be used to distribute workloads evenly across multiple consumers, allowing you to scale your application horizontally and handle increased traffic.

Buffering and Throttling: SQS can be used to buffer and throttle requests, allowing you to handle bursty traffic and protect against overloading your backend systems.
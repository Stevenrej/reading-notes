AWS API Gateway Overview

What is Amazon API Gateway?

- Amazon API Gateway is a fully managed service that makes it easy for developers to create, publish, maintain, monitor, and secure APIs at any scale. It allows you to create APIs that access AWS or other web services, as well as data stored in the AWS Cloud.

Why is Amazon API Gateway an important part of the Serverless ecosystem?

- PI Gateway is an important part of the Serverless ecosystem because it allows you to build and deploy APIs that can be triggered by events in other AWS services, such as a new object being created in an Amazon S3 bucket or an HTTP request being made to a custom API endpoint. This enables you to build and deploy Serverless applications that can scale to meet the needs of your users.

How does API Gateway integrate with other AWS services?

- API Gateway integrates with other AWS services through the use of custom integrations and Lambda functions.

AWS API Gateway

What are the some benefits of using Amazon API Gateway?

- Secure: API Gateway provides built-in security features, such as SSL/TLS and OAuth support, to help protect your APIs.
Customizable: API Gateway allows you to customize the behavior of your APIs through the use of custom integrations and Lambda functions.


What two API types might you choose from?

- REST APIs and HTTP APIs

AWS DynamoDB Guide

What is DynamoDB?

- DynamoDB is a fully managed NoSQL database service offered by AWS. It is designed for low-latency and high-throughput applications and can handle millions of requests per second with sub-millisecond response times.

Under what circumstances would you recommend DynamoDB over MongoDB?

- I would recommend DynamoDB over MongoDB in situations where you need a highly scalable, highly available database that can handle a large volume of read and write requests.


Dynamoose

What is Dynamoose?

- Dynamoose is an object modeling library for Node.js that provides a simple, intuitive interface for working with DynamoDB. It is designed to make it easier to work with DynamoDB by abstracting away some of the complexities of the DynamoDB API and providing a more familiar, MongoDB-like syntax.


What are some key features of Dynamoose?

- Schema support: Dynamoose allows you to define schemas for your data, which can help you enforce data integrity and make it easier to work with your data.
Validation: Dynamoose provides built-in support for validating data before it is saved to DynamoDB.
Index support: Dynamoose allows you to create secondary indexes on your data to support more efficient querying.

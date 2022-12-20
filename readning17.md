AWS S3

What is Amazon S3?

- Amazon S3 (Simple Storage Service) is an object storage service that offers industry-leading scalability, data availability, security, and performance. It is designed to store and retrieve any amount of data from anywhere on the internet.

2. Name some use cases for Amazon S3.

- 

Storing and backing up data: Amazon S3 can be used to store and protect a wide range of data types, including documents, images, videos, and audio files.


Serving static web content: Amazon S3 can be used to host static websites, such as blogs or marketing websites.


Storing data for analytics: Amazon S3 can be used to store data for analysis by tools such as Amazon Redshift, Amazon EMR, or Amazon Athena.





3. Name some benefits of using Amazon S3.

- 

Scalability: Amazon S3 can scale to store and serve billions of objects, making it suitable for storing and serving large amounts of data.

Data durability: Amazon S3 stores data across multiple devices in multiple facilities, and is designed to be highly durable with a 99% annual durability rate.

Security: Amazon S3 offers various security features, such as encryption and access control, to help protect data stored in the service.

AWS Lambda Basics

What is AWS Lambda?

- AWS Lambda is a cloud-based service that allows you to run code in response to events or in a fully managed environment. You can use AWS Lambda to build applications that automatically scale and respond to changing demand, without the need to provision or maintain infrastructure.

2. Name some use cases for AWS Lambdas.

running backend tasks in response to events, such as data updates or user actions.

Processing data streams in real-time, such as logs or data from IoT devices.

Building serverless APIs and microservices.




3. Describe “serverless” to a non-technical friend.

- "Serverless" refers to the concept of building and running applications without the need to worry about infrastructure. With a serverless approach, you can focus on writing and deploying code, while the cloud provider takes care of the underlying infrastructure and scaling. This can help you to reduce costs and increase flexibility, as you only pay for the resources you use and do not need to maintain any servers.

CDN

What is a CDN?

- A CDN (Content Delivery Network) is a distributed network of servers that are used to deliver web content to users based on their geographic location. CDNs work by replicating content from a website and storing it on servers located in various locations around the world. When a user requests content from a website that is using a CDN, the CDN will serve the content from the server that is closest to the user's location.

2. How does a CDN work with relation to the website visitor?

 - In terms of how a CDN works with relation to the website visitor, the process is typically transparent to the user. When a user accesses a website that is using a CDN, they will typically request the content from the website's domain name. The CDN will then intercept the request and serve the content from the nearest server. The user will receive the content as if it were being delivered directly from the website's server.

3. What are the benefits of employing a CDN?

Improved performance: By serving content from a server that is closer to the user, a CDN can help to reduce the time it takes for the content to be delivered, leading to a faster and more responsive user experience.

Increased scalability: A CDN can help to reduce the load on a website's server by offloading some of the content delivery to the CDN servers. This can help the website to scale to handle higher levels of traffic.

Improved security: CDNs often include security features such as DDoS protection, which can help to protect a website from malicious attacks.
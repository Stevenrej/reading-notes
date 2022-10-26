# API Design Best Practices

1. What does REST stand for? - Representational State Transfer
2. REST APIs are designed around a ____. - REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.
3. What is an identifier of a resource? Give an example. - A resource has an identifier, which is a URI that uniquely identifies that resource. https://adventure-works.com/orders/1
4. What are the most common HTTP verbs? - POST, GET, PUT, PATCH, and DELETE
5. What should the URIs be based on? - represent an object, uniquely and permanently
6. Give an example of a good URI. - Clean URIs are one component of a clean website, and it is an important one. The majority of end-user access to the Internet involves a URI, and whether or not the user actually enters the URI, they are working with one nonetheless.
7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing? - because requiring multiple network calls will slow down an application
8. What status code does a successful GET request return? - 200 OK status code means that the request was successful
9. What status code does an unsuccessful GET request return? - If not valid, 400
10. What status code does a successful POST request return? - 200: OK.
11. What status code does a successful DELETE request return? - A 202 ( Accepted ) status code

[Back To 301 Notes](https://stevenrej.github.io/reading-notes/readingnotes301main)
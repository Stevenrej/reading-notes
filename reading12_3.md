
# Status Codes Based On REST Methods

In your own words, describe what each group of status code represents:

100’s = 100 Continue informational status response code indicates that everything so far is OK
200’s = indicates that the request has succeeded.
300’s = indicates that the request has more than one possible responses
400’s = the server cannot or will not process the request due to something that is perceived to be a client error
500’s = the server encountered an unexpected condition that prevented it from fulfilling the request.
What is a status code 202? The request has been accepted for processing, but the processing has not been completed.
What is a status code 308? the resource requested has been definitively moved to the URL given by the Location headers.
What code would you use if an update didn’t return data to a client? 204
What code would you use if a resource used to exist but no longer does? 405
What is the ‘Forbidden’ status code? 403


## Build A REST API With Node.js, Express, & MongoDB - Quick - First 20 minutes

Why do we need to pull our MongoDB database string out of our server and put it into our .env? - so it can be read by the front end
What is middleware? software that provides common services and capabilities to applications outside of what's offered by the operating system.
What does app.use(express.json()) do? parse the incoming requests with JSON payloads
What does the /:id mean in a route?  it's a dynamic route
What is the difference between PUT and PATCH? PUT is a method of modifying resource where the client sends data that updates the entire resource . PATCH is a method of modifying resources where the client sends partial data that is to be updated without modifying the entire data
How do you make a default value in a schema? You can specify a default value for an item using the default keyword.
What does a 500 error status code mean? the server encountered an unexpected condition that prevented it from fulfilling the request
What is the difference between a status 200 and a status 201? 200: “Everything is OK.” This is the code that is delivered when a web page or resource acts exactly the way it's expected to. 201: “Created.”

[Back To 301 Notes](https://stevenrej.github.io/reading-notes/readingnotes301main)
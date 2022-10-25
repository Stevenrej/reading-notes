# How I explained REST to my brother

1. Who is Roy Fielding? -He helped write the first web servers, that sent documents across the internet… and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser.
2. Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world? -  Every programming language, database, or other kind of system has a different way of talking about nouns. That's why the URL is so important. It let's all of these systems tell each other about each other's nouns.
3. What is the HTTP protocol that Fielding and his friends created? - is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an HTTP GET on the URL you typed in and back comes a web page.
4. What does a GET do? - GET requests to retrieve resource representation/information only
5. What does a POST do? -POST APIs to create new subordinate resources
6. What does PUT do? - PUT APIs primarily to update an existing resource (if the resource does not exist, then API may decide to create a new resource or not).
7. What does PATCH do? - HTTP PATCH requests are to make a partial update on a resource.



[Back To 301 Notes](https://stevenrej.github.io/reading-notes/readingnotes301main)
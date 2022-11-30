# Readings

## Review: ES6 Classes

1. Classes are a template for creating ____.

- Objects

2. Can a class declaration be hoisted?

- yes

3. How would you describe a constructor and contextual “this” to a non-technical friend?

- It is a place in the code that define's what a object should be and this can be used ro refer to what is inside of that constructor

## Using Express Routing

1. Within Express, what does routing refer to?

- refers to how an application’s endpoints (URIs) respond to client requests

2. What is the difference between a route path and a route method?

- A route method is derived from one of the HTTP methods, and is attached to an instance of the express class. While Route paths, in combination with a request method, define the endpoints at which requests can be made. Route paths can be strings, string patterns, or regular expressions.

3. When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

- With multiple callback functions, it is important to provide next as an argument to the callback function and then call next() within the body of the function to hand off control to the next callback.

## Express Routing

1. What is an Express Router?

- Router is like a mini-Express application. It doesn’t bring in views or settings but provides us with the routing APIs like .use, .get, .param, and route.

2. By what mean do we initialize express.Router() in an express server?

- express.Router()

3. What do we use route middleware for?

- Route middleware in Express is a way to do something before a request is processed.

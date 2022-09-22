# Reading Notes 9

## HTML Forms

## Your first Web Form. How To Structure A Web Form

1. Why are forms so important in web development? - They are one of the main points of interaction between a user and the website/application

2. When designing a form, what are some key things to keep in mind when it comes to user experience? - What is the user experience going to be? Prioritizing Scannability And Readability

3. List 5 form elements and explain their importance. <form> <fieldset> <legend> <label> <input>

## Learn JS

## Introduction To Events

1. How would you describe events to a non-technical friend? - An event is like when you are in a room and people are talking and you here someone say your name you recognize that and know to listen to that event and follow the path

2. When using the addEventListener() method, what 2 arguments will you need to provide? - click and the function name

3. Describe the event object. Why is the target within the event object useful? - It provides extra features and info to the event handler, it designates where the event will take place

4. What is the difference between event bubbling and event capturing? - in the capturing phase The browser checks to see if the element's outer-most ancestor (<html>) has a click event handler registered on it for the capturing phase, and runs it if so.
Then it moves on to the next element inside <html> and does the same thing, then the next one, and so on until it reaches the direct parent of the element that was actually clicked.

while in the bubbling phase The browser checks to see if the direct parent of the clicked element has a click event handler registered on it for the bubbling phase, and runs it if so.
Then it moves on to the next immediate ancestor element and does the same thing, then the next one, and so on until it reaches the <html> element.

[Back To 201 Notes](https://stevenrej.github.io/reading-notes/readingnotes201main)

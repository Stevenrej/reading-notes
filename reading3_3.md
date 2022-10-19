# Reading

## React Docs - lists and keys

1. What does .map() return? -  a map object(which is an iterator) of the results after applying the given function to each item of a given iterable (list, tuple etc.) Syntax : map(fun, iter) Parameters : fun : It is a function to which map passes each element of given iterable.

2. If I want to loop through an array and display each value in JSX, how do I do that in React? - Use the map() method to iterate over the array

3. Each list item needs a unique . - Key

4. What is the purpose of a key? - help React identify which items have changed, are added, or are removed.

## The Spread Operator

1. What is the spread operator? - takes in an iterable (e.g an array) and expands it into individual elements.

2. List 4 things that the spread operator can do. - 

3. Give an example of using the spread operator to combine two arrays. - Copying an array.
Concatenating or combining arrays.
Using Math functions.
Using an array as arguments.

4. Give an example of using the spread operator to add a new item to an array. - Spread syntax "expands" an array into its elements

5. Give an example of using the spread operator to combine two objects into one. - The Object.assign() method allows you to copy all enumerable own properties from one or more source objects to a target object, and return the target object

## Videos

## How to Pass Functions Between Components

1. In the video, what is the first step that the developer does to pass functions between components? - create two components, one parent and one child.

2. In your own words, what does the increment function do? - determines the next node at the same level.

3. How can you pass a method from a parent component into a child component? - 1) Passing method as a prop using the arrow function : 2) Handling the passed function as a prop with the help of another function :

4. How does the child component invoke a method that was passed to it from a parent component? - Wrap the Child component in a forwardRef .
Use the useImperativeHandle hook in the child to add a function to the Child .
Call the Child's function from the Parent using the ref, e.g. childRef. current. childFunction() .

[Back To 301 Notes](https://stevenrej.github.io/reading-notes/readingnotes301main)
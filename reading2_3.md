React lifecycle

1. Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’? -  componentDidMount()

2. What is the very first thing to happen in the lifecycle of React? - static getDerivedStateFromProps()

3. Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates - componentDidMount, React Updates  componentWillUnmount constructor render

4. What does componentDidMount do? - allows us to execute the React code when the component is already placed in the DOM (Document Object Model)

React State Vs Props

1. What types of things can you pass in the props? - objects, arrays, and functions

2. What is the big difference between props and state? - Props are used to pass data from one component to another. The state is a local data storage that is local to the component only and cannot be passed to other components.

3. When do we re-render our application? -  schedules a render every time the state of a component changes

4. What are some examples of things that we could store in state? - data which may be a string , number or any complex object .

[Back To 301 Notes](https://stevenrej.github.io/reading-notes/readingnotes301main)
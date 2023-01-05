# Reading 29

## useReducer hook

1. Name an alternative to the useState Hook. - An alternative to the useState Hook is the useReducer Hook.
2. Why might the useReducer Hook be preferable to the useState Hook? - The useReducer Hook might be preferable to the useState Hook when you have complex state logic that involves multiple sub-values or when the next state depends on the previous state.
3. What are two ways to set the initial state? - Two ways to set the initial state are to specify it as an argument to the hook call and to specify it inside the reducer function.

## Ultimate Guide to useReducer

1. In terms of state, what does useReducer expect to receive as a parameter? - useReducer expects to receive a reducer function and an initial state as parameters.
2. What does useReducer return? - useReducer returns the current state and a dispatch function.
3. Explain dispatch to a non-technical recruiter. - Dispatch is a function that allows you to trigger an update to the current state. It works by taking an action object as an argument, which describes the update you want to make. The dispatch function then passes the action object to the reducer function, which uses it to calculate the next state.
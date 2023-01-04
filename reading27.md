# Reading 27

## Introducing Hooks

1. What was the motivation for introducing Hooks?
- The motivation for introducing Hooks was to provide a way for function components to have access to state and other React features without the need to convert the function component to a class component.

2. What changes are important regarding implementing Hooks versus Component Classes? - When implementing Hooks, there is no need to create a class or extend from a base component class. Instead, you can use Hooks directly in your function components.

3. Hooks allow you to reuse stateful logic without changing ___ _______. - Hooks allow you to reuse stateful logic without changing the structure of your component hierarchy.

hooks api

1. Name two rules imposed by React Hook usage.
- Two rules imposed by React Hook usage are: (1) Only call Hooks from the top level of your function components, and (2) Only call Hooks from within React function components or from custom Hooks. 

2. How would you identify a custom Hook and why might you create one? - You can identify a custom Hook by the fact that it has the word "use" at the beginning of its name. You might create a custom Hook to reuse stateful logic that is related to a specific feature in your app.

the state hook

1. What is a Hook? - The useState Hook is a built-in React Hook that allows you to add state to a function component.
2. When would I use the useState Hook? - You would use the useState Hook when you want to add state to a function component.

3. If you were to add React state to a function component by declaring a state variable:
1. What does calling useState do? - Calling useState declares a state variable for the function component.
2. What do we pass to useState as an argument? - You pass an initial state value to useState as an argument.

3. What does useState return? - useState returns a pair of values: the current state value and a function that can be used to update the state value.
# reading 28

1. What purpose does useEffect serve in a function component compared to its counterpart(s) in class components?

- The purpose of the useEffect hook is to allow a function component to perform side effects, such as making an API call or subscribing to an event. It serves a similar purpose as the componentDidMount, componentDidUpdate, and componentWillUnmount lifecycle methods in class components.

2. When using the useEffect Hook:

    1. What does useEffect do? - The useEffect hook is a function that takes in two arguments: a function to be run after the component renders, and an array of dependencies. It is called after the component renders, and will run the provided function. If the array of dependencies is provided, the hook will only run the function if one of the dependencies has changed.

    2. Why is useEffect called inside a component? - The useEffect hook is called inside a component because it is a way to allow the component to perform side effects. It is a way for the component to interact with the outside world and to update itself based on changes in the environment.

3. Explain the importance of properly implementing effects with Cleanup

- It is important to properly implement effects with cleanup because it helps to prevent memory leaks and unintended behavior. This can be done by returning a function from the effect that performs any necessary cleanup, such as canceling an API request or unsubscribing from an event. Properly implementing effects with cleanup helps to ensure that the component behaves as intended and does not cause any issues in the application.

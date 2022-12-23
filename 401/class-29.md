# Class 1

[401 Home](../home401.md)

## Advanced State with Reducers

### useReducer Hook

1. Name an alternative to useState Hook. useReducer!
2. Why might the useReducer Hook be preferable to the useState Hook? Where state logic is complex and involves multiple sub-values or when the next state depends on the previous one. It allows you to optimize performance  for components that trigger updates because you can pass dispatch down instead of callbacks.
3. What are two ways to set the initial state? State can be passed as the second argument to useReducer, or use the init function as the third argument. The state will be set to the argument passed to the init function, allowing the initial state to be derived elsewhere.

### Ultimate Guide to useReducer

1. In terms of state, what does useReducer expect to receive as a parameter? Both the reducer function and initial state.
2. What does useReducer return? An array of the current state and the dispatch function to invoke it later.
3. Explain dispatch to a non-technical recruiter. dispatch is a generic function that takes in the name of the action you'd like to have occur, and it will select from the options you've previously defined to have that option act.

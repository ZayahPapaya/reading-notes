# Class 1

[401 Home](../home401.md)

## Combined Reducers

### Multiple Reducers

1. Why create multiple reducers?
  Multiple reducers means separating the work and reading into different files similar to previous multi-level states while still managing them in one place.
2. How would you combine multiple reducers?
  const newReducer = combineReducers({reducer1: reducer1, reducer2: reducer2})
3. How will you manage state as an immutable object?
  Redux provides you the state for you to copy, edit the copy, and set the state as the edited state while still retaining a reference to the previous state(s)

### Redux Docs: Combined Reducers

1. combineReducers is a utility function to simplify the most common use case when writing Redux reducers.

2. Explain how combineReducers assembles the new state tree.
  combineReducers construccts a new grand object that contains the previous reducers using the name you set as a key and the value being the reducers passed in as arguments to combineReducers.

3. How would you define initial state in an app using combineReducers?
  1. The createStore function can take preloadedState as its second argument, which is intended for passing in a state that already exists elsewhere such as pulling from localStorage.
  
  2. The root reducer returns the initial state value when the state argument is undefined.

### Redux Docs: Syntax

1. Why will you want to split your reducing functions as your app becomes more complex?
  Each will manage their own parts of state separately while still being part of the larger Redux system.

2. The combineRReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.

3. What is a popular convention when naming reducers?
  Name reducers after the statee slices they manage so you can use ES6 property shorthand notation. ({banana: banana}) versues ({banana}).

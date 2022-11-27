# Class 1

[401 Home](../home401.md)

## Application State with Redux

1. What is the first principle of Redux?
  The entire state is represented as a single object. All changes are explicit and easily tracked.
2. What is a store and what do we use our reducers for within that store?
  The store is a shopping mall of actions to dispatch
3. Name three Redux store methods given to us by createStore and describe their use.
  getState() returns what the state looks like
  dispatch() dispatches an action from the store with arguments you give it to change state
  subscribe() sets a callback that is called each time an action is dispatched
4. Explain to a non-technical recruiter what combineReducers() does and why it is useful.
  combineReducers() constructs one big object for you to call reducers from without having to write it yourself, and with custom naming for each reducer set in it.
  
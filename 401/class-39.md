# Class 1

[401 Home](../home401.md)

## Redux - Additional

### RTK

1. What concerns are addressed by Redux Toolkit? Configuring Redux store is too complicated, Redux requires many packages to be useful, and Redux requires too much  boilerplate code.
2. What does  configureStore() do? Wraps createStore to provide simpplified config options and some good defaults. It can automatically combine slices, adds whatever middleware you supply, and includes thunks by default.
3. How would I use createSlice()? Pass in an object of reducer functions, a slice name, and the initial state of the slice. 

### MobX

1. What is Mobx? A state manager.
2. How does Mobx make it impossible to produce an inconsistent state? Everything that can be derived from the app state will be derived automatically.
3. How would we build a reactive user interface? The relevant store must be defined as observable to Mobx so that it watches for changes and updates states when they occur.

### Tutorial

1. What take-away(s) did this tutorial provide? Redux uses a bit of sleight of hand to provide mutable states in an indirect way, where you're actually mutating a draft state that will be used to write changes before the real state is updated to match appropriately.

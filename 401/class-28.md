# Class 1

[401 Home](../home401.md)

## Component Lifecycle / useEffect

1. What purpose does useEffect serve in a function component compared to its counterpart(s) in class components? Compared to componentDidMount and componentDidUpdate, useEffect doesn't block the browser from updating the screen. This makes the app feel more responsive.
2. When using the useEffect Hook:
  1. What does useEfffect do? Provide your function to React to invoke after the DOM updates.
  2. Why is useEffect called inside a component? useEffect can access the state due to being in the function scope.
3. Explain the importance of properly implementing effects with Cleanup. Without cleanup, your apap may have a memory leak.

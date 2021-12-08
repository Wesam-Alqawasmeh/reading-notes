# Class 29 Reading

---

**How can we ensure that an effect hook runs only once?**

- By passing empty array `([])` as a second argument after the call back function.

**Can useState() update more than one state variable at the same time?**

- If the state was an object when the state getting update it will delete the old object and it will take the new object value.

**Is useState() synchronous?**

- No, It is Asynchronous.

---

## Document the following Vocabulary Terms

**State Hook**: it is a special function that takes the initial state as an argument and returns an array of two entries.

**Component Lifecycle**: Each component in React has a lifecycle which you can monitor and manipulate during its three main phases. The three phases are: Mounting, Updating, and Unmounting.

![lifecycle](https://dev-to-uploads.s3.amazonaws.com/i/wh5rqu2bshfexy0w7g6a.png)

---

## useReducer hook

- An alternative to useState. Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method. (If you’re familiar with Redux, you already know how this works.)

- useReducer is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. useReducer also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.

# Class 37 Reading

---

**Why choose Redux instead of the Context API for global state?**

- Because, the React Context will trigger a re-render on each update, and optimizing it manually can be really tough.

**What is the purpose of a reducer?**

- a reducer is a pure function that takes an action and the previous state of the application and `returns the new state`. The action describes what happened and it is the reducer's job to return the new state based on that action.

**What does an action contain?**

- It contains the type that describes what will happen, and the payload for the new state.

**Why do we need to copy the state in a reducer?**

- because sometimes we need to back to the original state.

---

## Document the following Vocabulary Terms

**immutable state**: (unchanged state) any changes that need to be made to it within a function must be made to a copy of the state.

**time travel in redux**: it is the ability to move back and forth among the previous states of an application and view the results in real time.

**action creator**: it is a function that literally creates an action object.

**reducer**: it is a pure function that takes an action and the previous state of the application and returns the new state.

**dispatch**: dispatch an action. This is the only way to trigger a state change.

---

**More Materials about combine Reducers**

[Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

[Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)

[Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

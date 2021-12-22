## Class 39 Reading

---

**What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?**

- By calling an async action to fetch the data from our API inside useEffect() for function based component of componentDidMount for class based component.

**When using a thunk/async action that dispatches the actual action, which do you export from your reducer?**

- when the app needs to communicate with an external API or perform side effects.

---

## Document the following Vocabulary Terms

**middleware**: A function that we use to do some functionality or check of some data at the point we put it in the code.

**thunk**: is a programming concept where a function is used to delay the evaluation/calculation of an operation.

---

## Redux Toolkit

The Redux Toolkit package is intended to be the standard way to write Redux logic. It was originally created to help address three common concerns about Redux:

- "Configuring a Redux store is too complicated"
- "I have to add a lot of packages to get Redux to do anything useful"
- "Redux requires too much boilerplate code"

We can't solve every use case, but in the spirit of create-react-app and apollo-boost, we can try to provide some tools that abstract over the setup process and handle the most common use cases, as well as include some useful utilities that will let the user simplify their application code.

Redux Toolkit also includes a powerful data fetching and caching capability that we've dubbed "RTK Query". It's included in the package as a separate set of entry points. It's optional, but can eliminate the need to hand-write data fetching logic yourself.

These tools should be beneficial to all Redux users. Whether you're a brand new Redux user setting up your first project, or an experienced user who wants to simplify an existing application, Redux Toolkit can help you make your Redux code better.

# Class 38 Reading

---

**How granular should your reducers be?**

- For those parts which require different handling in various reducers; dedicated action is the best solution. For others, sometimes a general action might be good enough.

**Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched**

- it is a Pro more than a Con since we have to change multiple states in multiple components, the fact that all the reducers can listen when the action is dispatched can reduce a lot of work, each reducer can provide a different logic to the same dispatcher.

**Name a strategy for preventing the above**

- Redux thunk

---

## Document the following Vocabulary Terms

**Store**: it is an immutable object tree in Redux. A store is a state container which holds the application's state.

**combined reducers**: helper function turns an object whose values are different reducing functions into a single reducing function you can pass to `createStore`.

---

## async actions

So far, all the data we've worked with has been directly inside of our React+Redux client application. However, most real applications need to work with data from a server, by making HTTP API calls to fetch and save items.

a Redux middleware can do anything when it sees a dispatched action: log something, modify the action, delay the action, make an async call, and more. Also, since middleware form a pipeline around the real store.dispatch function, this also means that we could actually pass something that isn't a plain action object to dispatch, as long as a middleware intercepts that value and doesn't let it reach the reducers.

Middleware also have access to dispatch and getState. That means you could write some async logic in a middleware, and still have the ability to interact with the Redux store by dispatching actions.

## Redux Async Data Flow

So how do middleware and async logic affect the overall data flow of a Redux app?

Just like with a normal action, we first need to handle a user event in the application, such as a click on a button. Then, we call dispatch(), and pass in something, whether it be a plain action object, a function, or some other value that a middleware can look for.

Once that dispatched value reaches a middleware, it can make an async call, and then dispatch a real action object when the async call completes.

![async data flow](https://d33wubrfki0l68.cloudfront.net/08d01ed85246d3ece01963408572f3f6dfb49d41/4bc12/assets/images/reduxasyncdataflowdiagram-d97ff38a0f4da0f327163170ccc13e80.gif)

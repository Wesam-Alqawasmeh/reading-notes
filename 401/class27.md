# Class-27 Reading

---

**How does React differ from vanilla JS/HTML/CSS?**

1. Plain JS apps usually start with the initial UI created on the server (as HTML), whereas React apps start with a blank HTML page, and dynamically create the initial state in JavaScript.
2. React requires you to break your UI into components, but plain JS apps can be structured in any way you see fit.
3. Data for plain JS apps are stored in the DOM itself and has to be found from the DOM before it can be used. React apps store data in regular JavaScript variables
4. UI updates in plain JS have to happen by finding the DOM node to update and manually appending or removing elements. React automatically updates the UI based on setting and changing state within the component.

**What is the primary difference between a function component and a class component?**

- use a Hook inside the existing function component to manage the state and no need to convert it into the Class component. Instead of Classes, one can use Hooks in the Functional component as this is a much easier way of managing the state. Hooks can only be used in functional components, not in-class components.

---

## Document the following Vocabulary Terms

**Functional Components**: they are simply JavaScript functions that takes props and uses hooks in react.

**Children / Child Components**: components that are inside another components.

---

## State Hook

- useState is a Hook (we’ll talk about what this means in a moment). We call it inside a function component to add some local state to it. React will preserve this state between re-renders. useState returns a pair: the current state value and a function that lets you update it. You can call this function from an event handler or somewhere else. It’s similar to this.setState in a class, except it doesn’t merge the old and new state together. (We’ll show an example comparing useState to this.state in Using the State Hook.)

- The only argument to useState is the initial state. In the example above, it is 0 because our counter starts from zero. Note that unlike this.state, the state here doesn’t have to be an object — although it can be if you want. The initial state argument is only used during the first render.

- The array destructuring syntax lets us give different names to the state variables we declared by calling useState. These names aren’t a part of the useState API. Instead, React assumes that if you call useState many times, you do it in the same order during every render.

![hooks](https://cloudreports.net/wp-content/uploads/2019/06/react-hook-concepts-1.png)

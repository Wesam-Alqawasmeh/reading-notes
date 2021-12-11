# Class 31 Reading

---

**Describe use cases useState() vs useReducer()**

- `useState()`:

1. JavaScript primitives as state
2. simple state transitions
3. business logic within your component
4. different properties that don't change in any correlated way and can be managed by multiple useState hooks
5. state co-located to your component
6. a small application

- `useReducer()`:

1. JavaScript objects or arrays as state
2. complex state transitions
3. complicated business logic more suitable for a reducer function
4. different properties tied together that should be managed in one state object
5. the need to update state deep down in your component tree
6. a medium-sized application
7. need for an easier time testing it
8. need for a more predictable and maintainable state architecture

---

**Why do custom hooks need the use prefix?**

- Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.

**What do custom hooks usually do?**

- allow us to have cleaner functional components, remove logic from the UI layer, and prevent code duplication by bringing common use cases to reusable hooks.

**Using any list of custom hooks, research and name one that you think will be useful in your applications**

- useArray hook: providing us with various array manipulation methods. This hook is a part of the `react-hanger package`.

---

## Document the following Vocabulary Terms

**reducer**: it is a pure function that takes an action and the previous state of the application and returns the new state

---

## context api

- Context provides a way to pass data through the component tree without having to pass props down manually at every level.

**When to Use Context**

Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language. For example, in the code below we manually thread through a “theme” prop in order to style the Button component:

    class App extends React.Component {
    render() {
        return <Toolbar theme="dark" />;
    }
    }

    function Toolbar(props) {
    // The Toolbar component must take an extra "theme" prop
    // and pass it to the ThemedButton. This can become painful
    // if every single button in the app needs to know the theme
    // because it would have to be passed through all components.
    return (
        <div>
        <ThemedButton theme={props.theme} />
        </div>
    );
    }

    class ThemedButton extends React.Component {
    render() {
        return <Button theme={this.props.theme} />;
    }
    }

Using context, we can avoid passing props through intermediate elements:

    // Context lets us pass a value deep into the component tree
    // without explicitly threading it through every component.
    // Create a context for the current theme (with "light" as the default).
    const ThemeContext = React.createContext('light');

    class App extends React.Component {
    render() {
        // Use a Provider to pass the current theme to the tree below.
        // Any component can read it, no matter how deep it is.
        // In this example, we're passing "dark" as the current value.
        return (
        <ThemeContext.Provider value="dark">
            <Toolbar />
        </ThemeContext.Provider>
        );
    }
    }

    // A component in the middle doesn't have to
    // pass the theme down explicitly anymore.
    function Toolbar() {
    return (
        <div>
        <ThemedButton />
        </div>
    );
    }

    class ThemedButton extends React.Component {
    // Assign a contextType to read the current theme context.
    // React will find the closest theme Provider above and use its value.
    // In this example, the current theme is "dark".
    static contextType = ThemeContext;
    render() {
        return <Button theme={this.context} />;
    }
    }

## Class 28 Reading

---

**Why do we not need more .html pages in a multi-page React app?**

- Because we will use react router and this will manage all of the pages in one html page.

**If we wanted a component to show up on every page, where would we put it and why?**

    - Inside the <BrowserRouter />, outside a <Route />

**What does routing do with the components that were rendered when a new route is requested**

- It will stop the rendering of the old one, then It will render the requested components.

**What does props.children contain?**

- it is used to display whatever you include between the opening and closing tags when invoking a component.

**How do useState() and this.setState() differ?**

- useState() changes all of the state but this.setState() changes only what we passed to change.

---

## Document the following Vocabulary Terms

**State Hook**: It is a hook in react used with functional based components .

**Mounting and Un-Mounting**: Mounting means when the components is rendering, un mounting when the component is not rendering.

---

## effects hook

- By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates. In this effect, we set the document title, but we could also perform data fetching or call some other imperative API.

- Placing useEffect inside the component lets us access the count state variable (or any props) right from the effect. We don’t need a special API to read it — it’s already in the function scope. Hooks embrace JavaScript closures and avoid introducing React-specific APIs where JavaScript already provides a solution.

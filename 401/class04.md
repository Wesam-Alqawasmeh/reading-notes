# Data Modeling 

---

## Name 3 advantages to Test Driven Development

1. The software design becomes modular.

2. The code is easier to maintain and Code refactoring goes more smoothly.

3. Developers have less debugging to do and  Project costs descrease.

---

## In what case would you need to use beforeEach() or afterEach() in a test suite?

- In testing the console.log by implementing it before each test and resetting after each test.

---

## What is one downside of Test Driven Development

- You sometimes have to mock a lot of things or things that are difficult to mock. It’s beneficial in the long term, but painful right now.

- Hard to apply to existing legacy code.

- Unit testing is something the whole team has to buy into.

- Unless everyone on the team correctly maintains their tests, the whole system can quickly degrade.

---

## difference between ES6 Classes and Constructor/Prototype Classes

ES6 Classes | Constructor/Prototype Classes
----------------|----------------------
constructors creates objects by adding function to their prototypes | create objects along with inheritance property.
It ensures that this keyword used by the developer is referring to the object being created by the developer. | Any function can be used as a function constructor and it primarily focuses on the creation of reusable object creation code.
A child of an ES6 class is another type definition which extends the parent with new properties and methods, which in turn can be instantiated at runtime. | A child of a prototype is another object instance which delegates to the parent any properties that aren’t implemented on the child.


---

## Why REST?

1. REST is Easy to Understand and Implement.

2. REST Makes your Application More Scalable.

3. Caching is Easier with REST.

4. REST is Flexibile.


--- 


## Document the following Vocabulary Terms

- **functional programming**: is a declarative programming paradigm where programs are created by applying sequential functions rather than statements. Each function takes in an input value and returns a consistent output value without altering or being affected by the program state.

- **object-oriented programming (OOP)**: is a programming paradigm based on the concept of "objects", which can contain data and code: data in the form of fields (often known as attributes or properties), and code, in the form of procedures (often known as methods).

- **class**: a template for creating objects. It encapsulate data with code to work on that data.

- **super**: it is used to call the constructor of its parent class to access the parent's properties and methods.

- **this**: it is a keyword refers to the object it belongs to.

- **Test Driven Development (TDD)**: is a software development process relying on software requirements being converted to test cases before software is fully developed, and tracking all software development by repeatedly testing the software against all test cases.

- **Jest**: is a universal testing platform.

- **Continuous Integration (CI)**: is the practice of automating the integration of code changes from multiple contributors into a single software project. It’s a primary DevOps best practice, allowing developers to frequently merge code changes into a central repository where builds and tests then run.

- **REST**: REpresentational State Transfer, is an architectural style for providing standards between computer systems on the web, making it easier for systems to communicate with each other.

- **Data Model**: visual representations of an enterprise’s data elements and the connections between them. By helping to define and structure data.
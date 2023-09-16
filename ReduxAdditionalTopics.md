# Redux - Additional Topics
### Redux Toolkit (RTK)

**1.What concerns are addressed by Redux Toolkit?**

Redux Toolkit is a library that addresses several concerns in Redux applications to simplify and improve the development process:

* Boilerplate Reduction: It reduces the amount of repetitive and boilerplate code required to set up and manage Redux.

* Immutable State: Redux Toolkit promotes immutable state updates to prevent accidental mutations and common bugs.

* Action Creation: It simplifies the creation of actions and action creators, reducing naming inconsistencies and typos.

* Async Actions: Redux Toolkit seamlessly integrates with Redux Thunk middleware for handling asynchronous actions.

* DevTools Configuration: It automatically configures the Redux DevTools Extension for easier debugging.

* Performance Optimization: It offers memoized selectors for performance improvements.

* Encapsulation: Encourages grouping related actions and reducers together for better code organization.

* Type Safety: Redux Toolkit leverages TypeScript for improved type inference and type safety.


**2.What does configureStore() do?**
configureStore() is a function provided by Redux Toolkit that simplifies the process of creating a Redux store in a Redux application. It encapsulates several steps and configurations that are commonly used when setting up a Redux store, making it easier for developers to create a store with sensible defaults.

**3.How would I use createSlice()?**
Import Redux Toolkit
Create a Slice
Export Actions and Reducers
Use in a Reducer File

### MobX

**1.What is Mobx?**

MobX is a JavaScript state management library that is primarily used for managing the state of applications, particularly in user interfaces. It provides a simple and efficient way to handle the state of an application and keep it synchronized with the user interface. MobX stands for "Mobility of eXperience" and was inspired by reactive programming principles.

**2.How does MobX make it “impossible” to produce an inconsistent state?**
MobX makes it "impossible" to produce an inconsistent state by enforcing strict rules for state modification within actions, tracking dependencies, ensuring immediate updates, and providing safe mechanisms for observing changes. This strict adherence to reactivity principles helps maintain a consistent and predictable application state, reducing the likelihood of bugs and unexpected behavior caused by inconsistent state changes.

**3.How would we build a reactive user interface?**
To build a reactive user interface (UI) using MobX, you can follow these general steps:
Setup MobX
Define Your Application State
Create Actions
Derive Computed Values
Build Components
Inject State
Trigger Actions
React to State Changes
Cleanup


### Resources: 

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/introduction/getting-started)

[MobX](https://mobx.js.org/getting-started.html)

[Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

[HookState](https://hookstate.js.org/)


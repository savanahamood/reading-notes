# Redux - Combined Reducers

## Multiple Reducers Example

**1. Why create multiple reducers?**
using multiple reducers in Redux promotes a cleaner, more maintainable, and scalable codebase. It's a best practice that encourages good software engineering principles, such as modularity, separation of concerns, and reusability.

**2. How would you combine multiple reducers?** 

In Redux, you can combine multiple reducers into a single root reducer using Redux's built-in utility function called combineReducers. This allows you to manage different slices of your application's state separately and then combine them into a single state tree.
By combining multiple reducers with combineReducers, you can organize your Redux state management in a structured and modular way, making it easier to manage and scale your application.

**3. How will you manage state as an immutable object? why?** 
 managing state as an immutable object enhances predictability, simplifies debugging and testing, facilitates the use of pure functions, supports advanced debugging techniques, and aligns with best practices in modern web development. It contributes to a more maintainable and reliable codebase, especially in complex applications.


## Redux Docs: Using Combined Reducers

**1. combineReducers is a utility function to simplify the most common use case when writing ___ _____ .**
combineReducers

**2. Explain how combineReducers assembles the new state tree.**
combineReducers simplifies the process of managing different parts of your application's state by allowing you to delegate specific slices of the state to their respective reducers. It combines the individual state slices produced by these sub-reducers into a cohesive state tree, making it easier to manage and maintain complex state structures in your Redux application.

**3. How would you define initial state in an app using combineReducers?**
In an app using combineReducers in Redux:

* Create Reducers: Develop individual reducer functions, each responsible for managing a specific part of the application's state. Define an initialState variable within each reducer, specifying the initial values for that state slice.

* Combine Reducers: Use the combineReducers function to combine these individual reducers into a single root reducer. The root reducer orchestrates state management for the entire application.

* Accessing Initial State: If you need to access the initial state directly, import the individual reducer and access its initialState variable. This is typically done during initialization but is not commonly needed in components.

* Create the Redux Store: Create the Redux store using the root reducer. The store will contain the combined initial state for all slices defined by the individual reducers.

By following this approach, you can effectively set and manage the initial state for different slices of your application's state using combineReducers. Each reducer specifies its own initial state, and these initial states are consolidated into a single, unified initial state when creating the Redux store.


## Redux Docs: Combined Reducer Syntax

**1. Why will you want to split your reducing functions as your app becomes more complex?**

splitting reducing functions in a complex app enhances modularity, readability, testability, scalability, code reuse, debugging, collaboration, performance, and overall code maintainability. This approach promotes a more organized, manageable, and maintainable state management system as your application grows and evolves.


**2. The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____.**
The combineReducers helper function turns an object whose values are different reducing functions into a single reducing function you can pass to the Redux createStore function

**3. What is a popular convention when naming reducers?**
A popular convention when naming reducers in Redux is as follows:

* Use descriptive and meaningful names that clearly indicate the purpose or the part of the application state managed by the reducer.

* Utilize camelCase for naming, which involves starting each word with a capital letter except for the first word, which starts with a lowercase letter.

* Suffix the reducer function's name with "Reducer" to signify that it is a reducer responsible for state management (e.g., userReducer, postReducer).

* Avoid generic names like reducer1 and opt for specific, domain-related names that reflect the reducer's role in the application (e.g., userReducer, cartReducer).

* Group related reducers under a common directory or module structure to organize and clarify their association with specific features or data domains.




### Resources: 

[Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

[Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)

[Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

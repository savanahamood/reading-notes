# Application State with Redux

**1.What is the first principle of Redux?**

The first principle of Redux is "Single Source of Truth." This principle emphasizes that the entire state of your application is stored in a single JavaScript object, commonly referred to as the "store."

**2.what is a store and what do we use our reducers for within that store?**

 the store is the centralized place where your application's state is stored, and reducers are responsible for specifying how that state should change when actions are dispatched. Reducers help ensure that state changes are predictable, maintainable, and traceable. They play a crucial role in maintaining the "Single Source of Truth" principle in Redux.


**3.Name three Redux store methods given to us by createStore and describe their use.**

The createStore function in Redux provides several methods to interact with the store. Here are three essential methods provided by createStore and their uses:

1. getState():

Use: The getState() method is used to retrieve the current state of the Redux store.
* Description: When called, it returns the current state object, which represents the entire state tree of your application. You can access and read data from this state to display it in your components or perform any necessary operations.

2. dispatch(action):

Use: The dispatch(action) method is used to dispatch actions to the Redux store.
* Description: Actions are plain JavaScript objects that describe changes you want to make to the state. When you call dispatch(action), Redux processes the action through your reducers and updates the state accordingly. This is how you trigger state changes in your application.

3. subscribe(listener):

Use: The subscribe(listener) method is used to add listeners that will be notified whenever the state of the Redux store changes.
* Description: You pass a listener function to subscribe, and Redux will call this function whenever an action is dispatched and state changes occur. This allows you to react to state changes in your application, such as updating the user interface when the data in the store changes. The listener can be used to trigger re-renders in connected components.


**4.Explain to a non-technical recruiter what combineReducers() does and why it is useful.**

combineReducers() is like a project manager for your Redux state, ensuring that each part of your application's state is managed by the right team (reducer) and that everything works together smoothly. It's a valuable tool for building and maintaining complex applications with Redux.

### Resources:
 [Dan Abramov Redux Tutorials](https://egghead.io/courses/getting-started-with-redux)

[worlds easiest guide to redux](https://medium.freecodecamp.org/understanding-redux-the-worlds-easiest-guide-to-beginning-redux-c695f45546f6)

[testing reducers](https://medium.com/@netxm/testing-redux-reducers-with-jest-6653abbfe3e1)

[Redux Docs](https://redux.js.org/)
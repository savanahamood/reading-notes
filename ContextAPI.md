# Context API

### Choosing the State Structure

**1.Summarize the five principles for structuring state.**

1. Group related state. If you always update two or more state variables at the same time, consider merging them into a single state variable.
2. Avoid contradictions in state. When the state is structured in a way that several pieces of state may contradict and “disagree” with each other, you leave room for mistakes. Try to avoid this.
3. Avoid redundant state. If you can calculate some information from the component’s props or its existing state variables during rendering, you should not put that information into that component’s state.
4. Avoid duplication in state. When the same data is duplicated between multiple state variables, or within nested objects, it is difficult to keep them in sync. Reduce duplication when you can.
5. Avoid deeply nested state. Deeply hierarchical state is not very convenient to update. When possible, prefer to structure state in a flat way.



### Passing State Deeply with Context

**1.What problem do Contexts aim to solve?**
Context lets the parent component make some information available to any component in the tree below it—no matter how deep—without passing it explicitly through props.

**2.What is one technique to try before useContext?**
Prop Drilling

**3.What hook complements useContext for complex applications?**
useContext is great for accessing and subscribing to global state without prop drilling, it doesn't inherently handle complex state logic or state transitions. This is where useReducer comes in. It allows you to manage complex state changes and transitions in a more structured and predictable way.


### Resources:
 [Choosing the State Structure](https://react.dev/learn/choosing-the-state-structure)

[Passing State Deeply with Context](https://react.dev/learn/passing-data-deeply-with-context)

[Sharing State Between Components](https://react.dev/learn/sharing-state-between-components)

[Preserving and Restting State](https://react.dev/learn/preserving-and-resetting-state)

## Putting it all Together

### React Docs - Thinking in React

1. What is the single responsibility principle and how does it apply to components?
  - It means that each component should only do one thing, and if its purpose grows, it can be broken up into further sub-components that each handle only one thing.
2. What does it mean to build a ‘static’ version of your application?
- It renders the UI but is not interactive.
3. Once you have a static application, what do you need to add?
- Components that reuse other components and pass data using props.
4. What are the three questions you can ask to determine if something is state?
- Is it passed from a parent via props? - if so, probably not state
- Does it remain unchanged over time? - if so, probably not state
- Can you compute it based on any other state or props in your component? - if so it isn't state
5. How can you identify where state needs to live?
- Identify each component that renders something based on that state, find a common owner component, and either that common owner or a higher-level component should own the state.

### Higher-Order Functions

1. What is a “higher-order function”?
- Functions that operate on other functions, either by taking them as arguments or by returning them. They allow us to abstract over actions, not just values.
2. Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?
- It's a simplified arrow function with 'm' as a parameter and if 'm' > 'n'(the parameter for the greaterThan function), it will give a return value of true.
3. Explain how either map or reduce operates, with regards to higher-order functions.
- 

### Sources

[React Docs - Thinking in React](https://reactjs.org/docs/thinking-in-react.html)<br>
[Higher-Order Functions](https://eloquentjavascript.net/05_higher_order.html#h_xxCc98lOBK)<br>
## State and Props

### React Lifecycle

1.Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?  
- render happens first  

2.What is the very first thing to happen in the lifecycle of React?  
- Mounting is the first of three phases, the render phase is the first part of each of those three phases, and in the render part of the mounting phase, the constructor is what comes first.  

3.Put the following things in the order that they happen: componentDidMount, render, constructor, componentWillUnmount, React Updates  
- Constructor, render, componentDidMount, componentWillUnmount  

4.What does componentDidMount do?  
- I'm not totally clear on that even after reading that paragraph multiple times. It's a lifecycle method that gets invoked when a component is mounted (don't understand what mounting is either! I think it means updating the DOM with react).  


### React State vs. Props

1.What types of things can you pass in the props?  
- Things that you pass into a function, how you want it to render. When you want to display information inside of a function without hard coding it. The things you pass into a class constructor.  

2.What is the big difference between props and state?  
- Props are handled outisde of the component and passed into it. State is handled inside the component.  

3.When do we re-render our application?  
- When the state is changed inside the application  

4.What are some examples of things that we could store in state?  
- When you need to re-render and update your application based on user input. Form elements is an example.  


### Sources
[React Lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)<br>
[React State vs. Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)<br>
[React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)<br>
[React Docs - handling events](https://reactjs.org/docs/handling-events.html)<br>
[React Tutorial through 'Developer Tools'](https://reactjs.org/tutorial/tutorial.html)<br>
[React Bootstrap Documentation](https://react-bootstrap.github.io/)<br>
[Bootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)<br>
[Bootstrap Shuffle - a class "sandbox"](https://bootstrapshuffle.com/classes)<br>
[Netlify](https://www.netlify.com/)<br>
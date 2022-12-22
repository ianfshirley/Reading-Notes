## Introduction to React and Components

### Component-Based Architecture

1.What is a “component”?  
- It's a piece of code that has a clearly defined interface and conforms to recommended behavior of all components within an architecture. It is intended to interact with other components.  

2.What are the characteristics of a component?  
- Reusability − Components are usually designed to be reused in different situations in different applications. However, some components may be designed for a specific task.

- Replaceable − Components may be freely substituted with other similar components.

- Not context specific − Components are designed to operate in different environments and contexts.

- Extensible − A component can be extended from existing components to provide new behavior.

- Encapsulated − A A component depicts the interfaces, which allow the caller to use its functionality, and do not expose details of the internal processes or any internal variables or state.

- Independent − Components are designed to have minimal dependencies on other components.  
[Source: tutorialspoint.com](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)  

3.What are the advantages of using component-based architecture?    
- Components break up the UI into smaller pieces that are easy to use and understand.
- Being reusable saves time and effort, less lines of code to do the same thing. This also makes it easier to develop/build upon/maintain/evolve existing software without impacting other parts of the system.  
- Being independent makes the connectivity between them more flexible.  


### What is Props and How to Use it in React

1.What is “props” short for?  
- It's a keyword in React meaning 'properties'.   

2.How are props used in React?  
- Used to pass data from one component to another.  

3.What is the flow of props?  
- One-way, parent to child (vs. in JavaScript it goes both ways, up & down, child to parent and/or child to parent )

### Sources
[Component-Based Architecture](https://www.tutorialspoint.com/software_architecture_design/component_based_architecture.htm)  

[What is Props and How to Use it in React](https://itnext.io/what-is-props-and-how-to-use-it-in-react-da307f500da0)  

[React Tutorial through ‘Passing Data Through Props’](https://reactjs.org/tutorial/tutorial.html)  

[React Docs - Hello world](https://reactjs.org/docs/hello-world.html)  

[React Docs - Introducing JSX](https://reactjs.org/docs/introducing-jsx.html)  

[React Docs - Rendering elements](https://reactjs.org/docs/rendering-elements.html)  

[React Docs - Components and props](https://reactjs.org/docs/components-and-props.html)


## Passing Functions as Props

### React Docs - List and Keys

1.What does .map() return?  
- It returns a new array with the same number of items as the array that's passed into it as a parameter  

2.If I want to loop through an array and display each value in JSX, how do I do that in React?  
- use a .map() function with the array as a parameter, and the same array wrapped in curly braces within an `<li></li>` tag. Then put the name that function in curly brackets within a `<ul></ul>` tag.  

3.Each list item needs a unique ____.  
- key  

4.What is the purpose of a key?  
- They help React identify which items have changed, been added or removed. To give each element inside an array a stable identity.  


### The Spread Operator

1.What is the spread operator?  
- It's an ellipsis of three dots (...) used to expand an iterable object into the list of arguments  

2.List 4 things that the spread operator can do.  
- It can be used to pass an array into a JS function that's expecting separate arguments.  
- copy an array  
- concatenate of combine arrays  
- adding to state in React  
- combining objects  
- using Math functions  
- adding an item to a list  

3.Give an example of using the spread operator to combine two arrays.  
- `const array1 = [1, 2, 3]`
- `const array2 = [4, 5, 6]`
- `const combinedArray = [...array1, ...array2]`
- `console.log(...combinedArray); will display: 1, 2, 3, 4, 5, 6`  

4.Give an example of using the spread operator to add a new item to an array.    

- `const shortArr = [4, 5, 6]`
- `const longArr = [1, 2, 3, ...shorArr]`
- `console.log(longArr); will display: 1, 2, 3, 4, 5, 6`    

5.Give an example of using the spread operator to combine two objects into one.  
- `const objectOne = {hello: "🤪"}`
- `const objectTwo = {world: "🐻"}`
- `const objectThree = {...objectOne, ...objectTwo, laugh: "😂"}`
- `console.log(objectThree) // Object { hello: "🤪", world: "🐻", laugh: "😂" }`

### How to Pass Functions Between Components

1.In the video, what is the first step that the developer does to pass functions between components?  
- create an 'increment' function  

2.In your own words, what does the increment function do?  
- It updates the state of the component that it resides in, and because you sort of turn it into a props function, it allows you to update the state of another component from within another component.

3.How can you pass a method from a parent component into a child component?  
- I don't know. I watched the video 3 times and still don't know how to answer this question. It's late and I'm tired lol  

4.How does the child component invoke a method that was passed to it from a parent component?  
- I don't know. I watched the video 3 times and still don't know how to answer this question. It's late and I'm tired lol   


### Sources
[React Docs - Lists and Keys](https://reactjs.org/docs/lists-and-keys.html)  

[The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)  

[How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)  

[React Tutorial](https://reactjs.org/tutorial/tutorial.html)  

[React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)
## Data Structures & Algorithms

### Basic Recursion

- Base case - if this is true, no recursion
- Recursive case - if base case is not true, continue to re-call the function, looping until the recursive case is met.

### Data Structures you MUST know

- Linked List:
  - Consists of Nodes
  - Each Linked List has a 'head' property, the first node in the list
  - each Node has a value and a 'next' pointer (last Node points to 'null')
- Arrays:
  - a continuous block of cells in the computer memory
  - each item has a value and an index (its place in the array)
- Hash Table:
  - objects in JS
  - dictionaries in Python
  - it's like an array, but the memory location for each element doesn't need to be in the same place
- Stack and Queue:
  - stack = LIFO - has a top and each node has a next
  - queue = FIFO - has a front and rear and each node has a next
- Graphs and Trees:
  - graph: nodes pointing to other nodes. pointers are called edges. edges can have weight
  - tree: like a graph but data only expands out in one direction


### Why you should learn Big-O and stop hacking your way through algorithms

- The point of Big O is to find the most efficient way to do something, not just to show the efficiency of your algorithm. 

### Discussion Questions

1. What is 1 of the more important things you should consider when deciding which data structure is best suited to solve a particular problem?
- Big O. It's important to think about this before or while decicing which data structure to use for your algorithm, not just to determine the Big O for space and time after you've already written the algorithm. This is definitely something that is going to take some more practice, and will get easier the more familiar we become with different data structures.
2. How can we ensure that we’ll avoid an infinite recursive call stack?
- Have a base case, which when met will tell the function to exit the loop

### Sources

[Basic Recursion](https://www.youtube.com/watch?v=vPEJSJMg4jY)<br>
[Data Structures you MUST know](https://www.youtube.com/watch?v=sVxBVvlnJsM)<br>
[Big O Explained](https://www.youtube.com/watch?v=v4cd1O4zkGw)<br>
[8 Common Data Structures every Programmer must know](https://towardsdatascience.com/8-common-data-structures-every-programmer-must-know-171acf6a1a42)<br>
[Why you should learn Big-O and stop hacking your way through algorithms](https://triplebyte.com/blog/why-you-should-learn-big-o-and-stop-hacking-your-way-through-algorithms)<br>
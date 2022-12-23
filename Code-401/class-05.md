## Linked Lists

### Big O: Analysis of Algorithm Efficiency

- Big O notation is used to describe the efficiency of an algorithm or function. This is based on 2 factors:
  - Running Time (AKA time efficiency/complexity): the amount of time a function needs to complete
  - Memory Space (AKA space efficiency/complexity): the amount of memory resources a function uses to store data and instructions.
- The role of Big O is to describe the worst case of efficiency an algorithm can have in performing its job.
- 4 Key areas for analysis:
  1. Input Size
    - size of parameter values that are **read** by the algorithm
  2. Units of Measurement
    - Time:
      - time in milliseconds
      - number of operations executed
      - number of "Basic Operations" that are executed (the operation contributing most to total running time)
    - Space:
      - amount of space needed to hold the code for the algorithm
      - amount of space needed to hold the input data
      - amount of space needed for the output data
      - amount of space needed to hold the working space during calculation
  3. Orders of Growth
    - Constant Complexity Growth
    - Logarithmic Complexity Growth
    - Linear Complexity Growth
    - Linearithmic Complexity Growth
    - Quadratic Complexity Growth
    - Cubic Complexity Growth
    - Exponential Complexity Growth
    - Factorial Complexity Growth
  4. Best Case, Worst Case, Average Case (self explanatory)

![Basic Asymptotic Efficiency of Code](/img/EfficiencyNotations.png)


### Linked Lists

- A sequence of nodes that are connected/linked to each other. Each node references the next node in the link.

- Singly Linked Lists - only one reference, which points to the next node in a linked list
- Doubly Linked Lists - two references, one to the next and one to the previous node in a linked list

- Nodes: individual items/links that live in linked lists
- Head: reference to the first node in a linked list
- Current: reference to the node that is currently being looked at

- Traversal - foreach and for loops cannot be used to traverse through linked lists. We depend on the 'next' value in each node
  - The best way to approach traversal is with a while() loop, so you can check if the next node in the list is not null

- When constructing code with linked lists, it's a good idea to require that each node has a value.

### What's a Linked List, Anyway?

- Linked Lists are linear data structures. We traverse through nodes sequentially
- Arrays are static data structures - all resources must be allocated when the structure is created
- Linked lists are dynamic data structures - it can shrink and grow in memory
- Each node has two parts: the data/information it contains, and a reference to the next node
![Static Vs. Dynamic Memory Allocation](/img/LL.png)


### Sources

[Big O: Analysis of Algorithm Efficiency](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html)<br>
[Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)<br>
[What's a Linked List, Anyway?, Part 1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)<br>
[What's a Linked List, Anyway?, Part 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)<br>
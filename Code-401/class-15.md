## Implementation: Trees

- **Common Terminology:**
  - Node - a tree node is a component which may contain its own values, and references to other nodes.
  - Root - the root is the node at the beginning (top) of the tree
  - K - a number that specifies the max number of children any node may have in a k-ary tree. In a binary tree, `k=2`
  - Left - reference to one child node, in a binary tree
  - Right - reference to the other child node, in a binary treee
  - Edge - the edge in a tree is the link between a parent and child node
  - Leaf - a leaf is a node that does not have any children
  - Height - the height of a tree is the number of edges from the root to the furthest leaf

A Sample Tree:
![sample tree](/img/BinaryTree1.png)

**Depth First Traversal**
- Depth first traversal prioritizes going through the depth(height) of the tree first. There are several ways to carry out depth first traversal:
  - Pre-order: `root >> left >> right`
  - In-order: `left >> root >> right`
  - Post-order: `left >> right >> root`

![sample tree](/img/tree-example.png)

Given the sample tree above, our traversals would result in different paths:
- Pre-order: `A, B, D, E, C, F`
- In-order: `D, B, E, A, F, C`
- Post-order: `D, E, B, F, C, A`

- The most common way to tarverse through a tree is to use recursion. With these traversals, we rely on the call stack to navigate back up the tree when we have reached the end of a sub-path.

**Breadth First Traversal**

- Breadth first traversal iterates through the tree by going through each level of the tree, node-by-node horizontally. Given the same sample tree as above, the output would be:
  - `A, B, C, D, E, F`
- It usually uses a queue, instead of a call stack via recursion.
  - Enqueue the root node, the dequeue it and enqueue it's left (B) & right (C) nodes (in that order)
  - Now the root's left node (B) is at the front of the queue. Repeat the above process; dequeue the front, and enqueue it's left (D) and right (E) nodes.
  - Now the front is `C`. Dequeue it and enqueue it's left (E) and right (none) nodes.
  - When we reach a node that has no children (D is now at the front), we dequeue it without any further enqueue. (Dequeue D, E, & F)

- **K-Ary Trees**
 - Breadth first traversal works the same way as in a binary tree, but instead of left and right, it traverses through the level of the tree like a list of length 'k'.

 - **Adding a node**
  - There are no structural rules for where nodes are supposed to go in a binary tree.
  - One strategy is to fill all the child spots from the top down. To do so, we would leverage the use of breadth-first traversal. During traversal, find the first node that does not have all its children filled, and insert the new node as a child. We fill child slots from left to right.

- **Big O**
  - Big O time for inserting a new node is O(n). Searching for a specific node will also be O(n). Due to the lack of organization in binary trees, worst case will involve traversing the entire tree.
  - Big O space for node insertion using breadth first will be O(w), where 'w' is the largest width of the tree. (isn't this the same thing as O(n)?)

- **Binary Search Trees**
  - Binary search trees have the nodes organized so that all values smaller than the root are placed to the left, and all the nodes larger than the root are placed to the right.
  - This makes searching for a node faster, since you only have to search one side of the tree, and each level you go down, you only need to search one side of that node's children/descendents.
  - Big O time - O(h) h=height. The height of a balanced tree would be log(n), but worst case scenario is still O(n) if you need to traverse
  - Big O space would be O(1). Space needed does not increase with bigger trees.

### Sources

[Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)<br>
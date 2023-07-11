# Trees

 a "tree" is a data structure that resembles a hierarchical structure similar to a real-life tree. It consists of nodes connected by edges or links, where each node can have zero or more child nodes.

The topmost node in a tree is called the "root," and it serves as the starting point for traversing the tree. Each node in the tree, except for the root, has a parent node, and nodes that have a common parent are called "siblings." Nodes without children are called "leaves" or "leaf nodes."

### Common Terminology
Node - A Tree node is a component which may contain its own values, and references to other nodes
Root - The root is the node at the beginning of the tree
K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
Left - A reference to one child node, in a binary tree
Right - A reference to the other child node, in a binary tree
Edge - The edge in a tree is the link between a parent and child node
Leaf - A leaf is a node that does not have any children
Height - The height of a tree is the number of edges from the root to the furthest leaf



### There are various types of trees, each with its specific characteristics and purposes:

* Binary Tree: A binary tree is a tree in which each node has at most two children, referred to as the left child and the right child. This structure is used for efficient searching, sorting, and traversal algorithms.

* Binary Search Tree: A binary search tree (BST) is a binary tree with the property that the value of each node in the left subtree is less than or equal to its parent, and the value of each node in the right subtree is greater than its parent. BSTs are commonly used for efficient searching, insertion, and deletion operations.

* AVL Tree: An AVL (Adelson-Velskii and Landis) tree is a self-balancing binary search tree. It maintains a balance factor for each node, ensuring that the heights of the left and right subtrees differ by at most one. This balancing property allows for efficient operations on the tree.

* B-Tree: A B-tree is a balanced tree that is optimized for disk access. It is commonly used in file systems and databases, where large amounts of data need to be stored and retrieved efficiently.

### Sample Tree

![Queue Visualization](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/images/BinaryTree1.PNG
)

Traversals
An important aspect of trees is how to traverse them. Traversing a tree allows us to search for a node, print out the contents of a tree, and much more! There are two categories of traversals when it comes to trees:

* Depth First : is a traversal technique used to explore or visit all the nodes of a tree or graph data structure. It is called "Depth First" because it starts at the root node and explores as far as possible along each branch before backtracking.

Depth First traversal can be performed using different strategies:

1. Preorder Traversal: In Preorder traversal, the algorithm visits the current node before its children. It follows the order of "Root-Left-Right." The steps for Preorder traversal are:
a. Visit the current node.
b. Traverse the left subtree recursively using Preorder.
c. Traverse the right subtree recursively using Preorder.

2. Inorder Traversal: In Inorder traversal, the algorithm visits the left subtree, then the current node, and finally the right subtree. It follows the order of "Left-Root-Right." The steps for Inorder traversal are:
a. Traverse the left subtree recursively using Inorder.
b. Visit the current node.
c. Traverse the right subtree recursively using Inorder.

3. Postorder Traversal: In Postorder traversal, the algorithm visits the children of the current node before visiting the current node itself. It follows the order of "Left-Right-Root." The steps for Postorder traversal are:
a. Traverse the left subtree recursively using Postorder.
b. Traverse the right subtree recursively using Postorder.
c. Visit the current node.



* Breadth First : is another traversal technique used to explore or visit all the nodes of a tree or graph data structure. It explores the nodes in a level-by-level manner, visiting all the nodes at a particular level before moving on to the next level.

can be performed using the following steps:

1. Start by visiting the root node of the tree.
2. Enqueue the root node into a queue data structure.
3. While the queue is not empty, do the following:
a. Dequeue a node from the front of the queue.
b. Process the dequeued node (e.g., visit the node, perform a specific operation).
c. Enqueue all the children (if any) of the dequeued node into the queue.
4. Repeat steps 3a-3c until the queue is empty.

### Binary Tree Vs K-ary Trees
**Binary Tree:**
In a binary tree, each node can have at most two children, referred to as the left child and the right child.
The left child is usually smaller (according to a defined ordering) than the parent node, and the right child is greater.
The absence of a child is represented by a null value.
Binary trees are commonly used for efficient searching, sorting, and traversal algorithms.
Various binary tree variations include Binary Search Trees (BST), AVL Trees, and Red-Black Trees.


**K-ary Tree:**
In a K-ary tree, each node can have at most K children, where K is a positive integer greater than or equal to 2.
K-ary trees allow for more than two children per node, providing a higher degree of branching.
K-ary trees are used in scenarios where nodes have a variable number of children or when the number of children per node is known and fixed.
Special cases of K-ary trees include ternary trees (K = 3) and quaternary trees (K = 4).
The choice of using a binary tree or a K-ary tree depends on the specific requirements of the problem at hand. Binary trees are often used for efficient searching and sorting, while K-ary trees are more suitable when nodes have a higher degree of branching.

### Binary Search Trees
A Binary Search Tree (BST) is a type of tree that does have some structure attached to it. In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

#### Searching a BST
Searching a BST can be done quickly, because all you do is compare the node you are searching for against the root of the tree or sub-tree. If the value is smaller, you only traverse the left side. If the value is larger, you only traverse the right side.

### Resources: [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)
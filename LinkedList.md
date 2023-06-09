# Linked Lists
A linked list is a linear data structure that consists of a sequence of elements called nodes, where each node contains a value and a reference (or link) to the next node in the sequence. The last node in the list typically points to a null reference to indicate the end of the list.

![Look Like](LinkedList1.png)


### Traversal
When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing. The Next property is exceptionally important because it will lead us where the next node is and allow us to extract the data appropriately.
The best way to approach a traversal is through the use of a while() loop. This allows us to continually check that the Next node in the list is not null. If we accidentally end up trying to traverse on a node that is null, a NullReferenceException gets thrown and our program will crash/end.
When traversing through a linked list, the Current variable will tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end.


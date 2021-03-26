

# Linked Lists  

Linked Lists are nodes that are in a sequence. That is they are connected and each node references the next one in the link. 

- Linked List
  - A node that points to the next one in the chain
- Singly
  - Refers to the number of references that a node has. If its singly linked it only has 1 reference.
 - Doubly
  - Referes to a node that has two references
 - Node
  - Individual items that are in the linked list
 - Next
  - This property of the node contains the data for the next link
 - Head
  - Referes to the type reference for the first node 
 - Current
  - Is the reference type for the current node in the list





# What is a linked list Part 1

Linked Lists are Dynamic Data Structures. That means that they can shrink and grow in the memory.

As before Linked Lists are made up of nodes which are elements in the list. 
It always has a head or first node to point the rest where to go. The last element is a node that points to an empty value. 

Singly Linked Lists only have 1 reference point per node. Think of it that they travel down a one way street. 

Doubly Linked Lists have 2 reference points per node. This would be like a 2 way street. 

There are also circular linked lists where the ending node does not point to null but instead points back towards another node. 


# What is a linked list Part 2

Linked Lists have Big O notation. Linked Lists are O(1) as they always have a constant run time. This is fine for small lists but for large ones it may take time to run. 

If you are working with large data sets you may need to use arrays instead. 

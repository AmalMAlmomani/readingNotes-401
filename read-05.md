# Linked Lists
-  ![](linked.jpeg)
## What is a Linked List
   -  a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.
   -  A data structure that contains nodes that links/points to the next node in the list.

## two types of Linked List 
   - Singly and Doubly

   - **Singly linked list** means that there is only one reference, and the reference points to the Next node in a linked list.
   - **Doubly linked list** means that there is a reference to both the Next and Previous node.

## Nodes 
   - are the individual items/links that live in a linked list. Each node contains the data for each link.
## Next 
   - Each node contains a property called *Next*. This property contains the reference to the next node.
   - it will lead us where the next node is and allow us to extract the data appropriately.


## The Head
  - is a reference type of type Node to the *first node* in a linked list.
## The Current reference 
  - is a reference type of type Node that is currently being looked at. 
  - tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end.

### Singly Linked List

#### Traversal
   - When traversing a linked list, you are not able to use a foreach or for loop.
  - best way to approach a traversal is through the use of a while() loop.
    - check that the *Next* node in the list is *not null*.
    - *NullReferenceException* gets thrown and our program will crash/end.

    - **When constructing your code, a few things to keep in mind.**
      - When making your Node class, consider requiring a value to be passed in to require that each node has a value.

      - When making a Linked List, you may want to require that at least one node gets passed in upon instantiation. This first node is what your Head and Current will point too.



- ![](arrayvslinked.jpeg)
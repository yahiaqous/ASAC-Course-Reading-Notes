# Linked Lists

## What is a Linked List

**A Linked List** is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link.

**Nodes**: the individual items/links that live in a linked list. Each node contains the data for each link.

&nbsp;

### Types of Linked List:

- **Singly**: refers to the number of references the node has. A Singly linked list means that there is only one reference, and the reference points to the next node in a linked list.

- **Doubly**: refers to there being two (double) references within the node. A Doubly linked list means that there is a reference to both the Next and Previous nodes.

![LinkedList1](Pictures/LinkedList1.png)

&nbsp;

### Traversal Big O

The Big O of **time** for Includes would be **O(n)**. This is because, in its worse case, the node we are looking for will be the very last node in the linked list. n represents the number of nodes in the linked list.

The Big O of **space** for Includes would be **O(1)**. This is because there is no additional space being used than what is already given to us with the linked list input.

One characteristic of linked lists is that they are **linear data structures**, which means that there is a sequence and an order to how they are constructed and traversed

![LinearVSnonlinear](Pictures/LinearVSnonlinear.jpeg)

&nbsp;

### Memory management

The biggest differentiator between arrays and linked lists is the way that they use memory in our machines, arrays are static data structures, while linked lists are dynamic data structures

![MemoryAllocation](Pictures/MemoryAllocation.jpeg)

A **circular linked list** is a little odd in that it doesn’t end with a node pointing to a null value. Instead, it has a node that acts as the tail of the list, and the node after the tail node is the beginning of the list

a linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element.

![ArraysVSlinkedLists](Pictures/ArraysVSlinkedLists.jpeg)

&nbsp;

## Big O Notation

**Big O Notation** is a way to express the amount of time that a function, action, or algorithm takes to run based on how many elements are passed to that function.

There are two major points to consider when thinking about how an algorithm performs: how much time it requires at runtime given how much time and memory it needs.

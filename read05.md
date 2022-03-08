## Big O
Big O(oh) notation is used to describe the efficiency of an algorithm or function.
### evaluated based on 2 factors
1. Running Time
2. Memory Space
Big O’s role in algorithm efficiency is to describe the Worst Case of efficiency an algorithm can have in performing it’s job

### we should consider 4 Key Areas for analysis:

1. Input Size:
*Input Size refers to the size of the parameter values that are read by the algorithm.
2. Units of Measurement
* The time in milliseconds from the start of a function execution until it ends
* The number of operations that are executed.
Think of this as the number of lines of code that are executed from start to finish of a function.
* The number of “Basic Operations” that are executed.

### Always be aware that Space Complexity and Time Complexity are measured differently and should be analyzed separately.

We can describe overall efficiency by using the input size n and measuring the overall Units of Space and Time required for the given input size n. As the value of n

3. Orders of Growth
4. Best Case, Worst Case, and Average Case


# Linked Lists

A Linked List is a sequence of Nodes that are connected/linked to each other.

Linked List - A data structure that contains nodes that links/points to the next node in the list.
 the node like  a point  
 next :mean the next step 
 Head : The Head is a reference of type Node to the first node in a linked list.
 


### Traversal
When traversing a linked list, you are not able to use a foreach or for loop. We depend on the Next value in each node to guide us where the next reference is pointing.but we can use while 

### Adding a Node
If we want to add a node with an O(1) efficiency, we have to replace the current Head of the linked list with the new node, without losing the reference to the next node in the list.
### Linear data structures
we traverse through element sequesnsly 
### Memory management
The biggest differentiator between arrays and linked lists is the way that they use memory in our machines.

The fundamental difference between arrays and linked lists is that arrays are static data structures, while linked lists are dynamic data structures. A static data structure needs all of its resources to be allocated when the structure is created; this means that even if the structure was to grow or shrink in size and elements were to be added or removed, it still always needs a given size and amount of memory. 


### Parts of a linked list
A linked list can be small or huge, but no matter the size, the parts that make it up are actually fairly simple. A linked list is made up of a series of nodes, which are the elements of the list.

# Stacks and Queues
# the Stack
A stack is a data structure that consists of Nodes. Each Node references the next Node in the stack, but does not reference its previous.
1. push node to add 
2. pop to delet a node 
3. peek return the top node 
4. isEmty return true when its empty
## First In Last Out in the stack

## Push 
when we want to push an item 
the new node.next in the first =null
then we assighn the new node.next =top
then top = new node value 
## Pop is removing a node 
we declere new value temp=top
let it point to the top 

then top=top.next
change the top value to the next 
temp.next =null
then delet it by put the temp.next =null
## Peek 
return top.value 
## IsEmpty 
return true if top.value is null
# Queue
1. Enqueue - Nodes or items that are added to the queue.
2. Dequeue - Nodes or items that are removed from the queue.
3. Front - This is the front/first Node of the queue.
4. Rear - This is the rear/last Node of the queue.
5. Peek 
will return the value of front node 
6. IsEmpty - returns true when queue is empty otherwise returns false.

## First In First Out in the queue

## Enqueue function to add a node 
to add node wa change the rear.next in the que to the new node 
rear =the new node
## Dequeue function in queue
firstly chek if its not empty by isempty function

he first thing you want to do is create a temporary reference type named temp and have it point to the same Node that front is pointing too.
then assign front to front.next 
then temp.next =null

## Peek 
return the front but firstly make sure its not empty by isempty function 
## IsEmpty 
return true if front is null


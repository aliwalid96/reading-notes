# trees
1. Root - The root is the node at the beginning of the tree
2. K - A number that specifies the maximum number of children any node may have in a k-ary tree

3. Left - A reference to one child node, in a binary tree
4. Right - A reference to the other child node, in a binary tree
5. Edge - The edge in a tree is the link between a parent and child node
6. Leaf - A leaf is a node that does not have any children
7. Height - The height of a tree is the number of edges from the root to the furthest leaf
## Traversals
1. Depth First
Depth first traversal is where we prioritize going through the depth (height) of the tree first

Here are three methods for depth first traversal:
1. 1 Pre-order: root >> left >> right
~~~
ALGORITHM preOrder(root)

  OUTPUT <-- root.value

  if root.left is not NULL
      preOrder(root.left)

  if root.right is not NULL
      preOrder(root.right)
~~~
This means that we will output the root.value out to the console. Then, our next block of code instructs us to check if our root has a left node set. If the root does, we will then send the left node to our preOrder method recursively. This means that we make another function call, where B is our new root


1. 2In-order: left >> root >> right

~~~
ALGORITHM inOrder(root)
// INPUT <-- root node
// OUTPUT <-- in-order output of tree node's values

    if root.left is not NULL
        inOrder(root.left)

    OUTPUT <-- root.value

    if root.right is not NULL
        inOrder(root.right)

~~~
1. 3Post-order: left >> right >> root
~~~
ALGORITHM postOrder(root)
// INPUT <-- root node
// OUTPUT <-- post-order output of tree node's values

    if root.left is not NULL
        postOrder(root.left)

    if root.right is not NULL
        postOrder(root.right)

    OUTPUT <-- root.value
~~~



2. Breadth First

eadth first traversal iterates through the tree by going through each level of the tree node-by-node.

Given our starting tree shown above, let’s start by putting the root into the queue:



~~~
ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while ! breadth.is_empty()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    if front.left is not NULL
      breadth.enqueue(front.left)

    if front.right is not NULL
      breadth.enqueue(front.right)
~~~
## Binary Tree Vs K-ary Trees


Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).


If Nodes are able have more than 2 child nodes, we call the tree that contains them a K-ary Tree.
## Breadth First Traversal



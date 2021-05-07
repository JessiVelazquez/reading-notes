# Trees

[Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)

**Important Terms**

Node - A Tree node is a component which may contain it’s own values, and references to other nodes

Root - The root is the node at the beginning of the tree

K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.

Left - A reference to one child node, in a binary tree

Right - A reference to the other child node, in a binary tree

Edge - The edge in a tree is the link between a parent and child node

Leaf - A leaf is a node that does not have any children

Height - The height of a tree is the number of edges from the root to the furthest leaf

## **Depth First Traversal**

**Using Recursion:** Relying on the call stack to get back up the tree when we have reached the end of a path.

This is where you prioritize going the depth, or height, of the tree first.

  - Pre-order: the root has to be looked at first

    - When we call pre-order, the root will be pushed to the call stack

      1. Push root to call stack

      2. if roote has a left node set, send left to pre-order (assigns it as root)

      3. When we hit the end of the line (a leaf), the code will look left and right, and left and right will both return null, and the last node will be popped off the stack, assigning root back to the level above.

      4. It will then look right from the second level, go to the right branch, find the leaf and the same will happen - leaf is popped off the call stack, so root goes back up a level.

      5. Eventually all sub levels of this branch will become leaves, and be popped off the call stack, returning the root to the original root ("top" of the tree), and the algorithm will look in the other direction.

Pseudo Code:

```
ALGORITHM preOrder(root)
// INPUT <-- root node
// OUTPUT <-- pre-order output of tree node's values

    OUTPUT <-- root.value

    if root.left is not Null
        preOrder(root.left)

    if root.right is not NULL
        preOrder(root.right)
```

  - In-order

Psuedo Code:

```
ALGORITHM inOrder(root)
// INPUT <-- root node
// OUTPUT <-- in-order output of tree node's values

    if root.left is not NULL
        inOrder(root.left)

    OUTPUT <-- root.value

    if root.right is not NULL
        inOrder(root.right)
```

  - Post-order

```
ALGORITHM postOrder(root)
// INPUT <-- root node
// OUTPUT <-- post-order output of tree node's values

    if root.left is not NULL
        postOrder(root.left)

    if root.right is not NULL
        postOrder(root.right)

    OUTPUT <-- root.value
```

**The difference here is when you output the root**

## **Breadth First Traversal**

This uses a queue instead of a call stack

1. Put root into queue

2. Dequeue root from queue

3. Enqueue the left and right children

4. Now we have node B (second level) in front of queue.

5. Enqueue this node's left and right children

Continue this process of enqueue node, dequeue, enqueue its children, etc. When we hit nodes with no children, we just dequeue it without any enqueues. 

Psueodo Code:

```
ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while breadth.peek()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    if front.left is not NULL
      breadth.enqueue(front.left)

    if front.right is not NULL
      breadth.enqueue(front.right)
```

**Binary Tree:** restricts children to 2 per node - left and right

**K-ary Tree:** nodes can have any number of children and "k" value is the maximum per node

  - with a K-ary tree, we use the same breadth first system of queueing nodes, then dequeueing and processing them, followed by enqueuing the current node's children until the queue is empty of child nodes.

Pseudo Code:

```
ALGORITHM breadthFirst(root)
// INPUT  <-- root node
// OUTPUT <-- front node of queue to console

  Queue breadth <-- new Queue()
  breadth.enqueue(root)

  while breadth.peek()
    node front = breadth.dequeue()
    OUTPUT <-- front.value

    for child in front.children
        breadth.enqueue(child)
```

Again, the link here is great. Refer to the diagrams. No need to copy them all here: [https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)
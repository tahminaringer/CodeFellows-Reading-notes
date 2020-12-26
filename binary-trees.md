# Binary Trees

- **Tree** Is a non linear data structure
- **Binary Search Tree** Is a data structure that is a collection of nodes connected by some edges
  - **Node** - A node is the individual item/dat that makes up the data structure
  - **Root** The root is the first/top node in the tree
  - **Left Child**- The node that is positioned to the left of a root or node.
  - **Edge** - The edge in a tree is the link between a parent and child node
  - **Leaf** - A leaf is a node that does not contain any children
  - **Height** - The height of a tree is determined by the number of edges from the root to the bottommost node

## Traversals
  
### Depth First

- you prioritze going through the depth/height of the tree first

#### Ways to Traverse

- *Pre-Order* `root >> left >> right`

```js
  ALGORITHM preOrder(root)

  OUTPUT <-- root.value

  if root.left is not NULL
      preOrder(root.left)

  if root.right is not NULL
      preOrder(root.right)
```

- *In-Order* `left >> root >> right`

```js
    if root.left is not NULL
        inOrder(root.left)

    OUTPUT <-- root.value

    if root.right is not NULL
        inOrder(root.right)
```

- *Post-Order* `left >> right >> root`

```js

    if root.left is not NULL
        postOrder(root.left)

    if root.right is not NULL
        postOrder(root.right)

    OUTPUT <-- root.value
```

### Breadth First

- traversal iterates through the tree by going through each level of the tree node-by-node

```js
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

## Binary Trees

- trees can have any number of children per node
- no spceific sorting order and can be added where ever space allows

### Adding a node

- Since no structual rules it doesn't matter where new nodes get placed
- **Fill all Child spots from top down** - use breadth first traversal find first node that dose not have 2 child nodes and insert the new node as a child. Slots are filled from left to right

## Binary Search Tree

- Type of tree that does have some structure attached to it. 
  - Nodes are organized in a manner where all values that are smaller that the root are placed to the left and all values that are larger than the root are placed to the right
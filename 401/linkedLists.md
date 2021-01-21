# Linked Lists

- **Linked List** sequence of Nodes that are connected to eachother. Each node references to the next node in the link.
  - Singly - refers to the number of references the node has
  - Doubly - refers to there being two references within the node - Next and previous
  - Node - individual items that live in linked list and contain the data for each link
  - Next each node contains a prperty called next and references the next node
  - Head - is a reference type of type `Node` to the first node in a linked list
  - Current - reference type of type that is currently being looked at
- Cannot use forEach or for loop instead depend on `next` and `while()`
- linear data structures

## Big O 

- `O(1)` takes constant time, doesnt matter how many elements we have or how huge our input is.
- `O(n)` linear, as our input grows the space and time that we need to run algorithm grows linearly
- `O(2)` takes exponentially more time and memory the more elements that your have. AVOID

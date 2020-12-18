# Stacks & Queues

- **Stack** is a data structure that consists of Nodes.
  - Each Node references the next Node in the stack but does not reference its previous

## Common Terminaology for stack

- `Push` Nodes or item that are put into the stack are pushed
- `Pop` Nodes or items that are removed form the stack are popped.
  - When you attemt to pop an empty stack an exception will be raised
- `Top` this is the top of the stack
- `Peek` When you peek you will view the value of the top Node in the stack
  - When you attempt to peek an empty stack an ecveption will be raised.
- `IsEmpty` returns true when stack is empty otherwise returns false

`FILO` First In Last Out - This means that the first item added in the stack will be the last item popped out of the stack

`LIFO` - Last in First out - This means that the last item added to the stack will be the first item popped out of the stack

`Push O(1)` Pushing a Node onto a stack will always be and o(n) Because it will allways take the same amount of time no matter how many nodes you have in the stack

`Pop O(1)` Popping a node off a stack is the action of removing a node from the top. when poping the node will be re-asigned  to the node that lives below and the top node isreturned to the user

`Peek O(1)` When coducting a peek you will only be inspecting the top node of the stack .  Typically you would chek `isEmpty` before conducting peek

`IsEmpty O(1)` 

```js
ALGORITHM isEmpty()
// INPUT <-- none
// OUTPUT <-- boolean

return top = NULL
```

## What is a Queue

- Enqueue - Nodes or items that are added to the queue. 0(1)
- Dequeue - Nodes or items that are removed from the queue. If called when the queue is empty an exception will be raised.
- Front - This is the front/first Node of the queue.
- Rear - This is the rear/last Node of the queue.
- Peek - When you peek you will view the value of the front - Node in the queue. If called when the queue is empty an exception will be raised.
- IsEmpty - returns true when queue is empty otherwise returns false.

`FIFO` Fist In First Out - This means that the first item in the queue will be the first item out of the queue

`LILO` Last In Last Out - This means that the last item in the queue will be the last item out of the queue

```js
ALGORITHM enqueue(value)
// INPUT <-- value to add to queue (will be wrapped in Node internally)
// OUTPUT <-- none
   node = new Node(value)
   rear.next <-- node
   rear <-- node
   ```
```js
ALGORITHM dequeue()
// INPUT <-- none
// OUTPUT <-- value of the removed Node
// EXCEPTION if queue is empty

   Node temp <-- front
   front <-- front.next
   temp.next <-- null

   return temp.value
   ```

```js
ALGORITHM peek()
// INPUT <-- none
// OUTPUT <-- value of the front Node in Queue
// EXCEPTION if Queue is empty

   return front.value
```

```js

ALGORITHM isEmpty()
// INPUT <-- none
// OUTPUT <-- boolean

return front = NULL
```

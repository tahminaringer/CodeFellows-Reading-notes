# Graphs

- non-linear data structure/collection of vertices or nodes, connected by line segments named edges

## Terminology

- **Vertex** also called node is a data object that can have 0 or mor adjacent vertices
- **Edge** an edge is a connection between two nodes
- **Neighbor** the neighbors of a node are its adjacent nodes/connected via an edge
- **Degree** The degree of vertex is the number of edges connected to that vertex
- **Undirected Grapp** graph where each edge is undirected or bi-directional/does not move in any direction
- **Directed Graphs or Digraph** is a graph where every edge is directed
- **Complete Graphs** all nodes are connected to all other nodes
- **Connected** has all of its vertices/nodes have atleast one edge
- **Disconnected** Where some vertices/nodes my not have edges
- **Acyclic Graph** Dirrected graph without cycles in other word a node connot be traversed and end up back at itself
- **Cycle Graphs** has cycles a node has a path back to itself
- **Weighted Graphs** graph with numbers assigned to its edges. Numbers are called `weights`
- **Breadth First Traversal**

```js

ALGORITHM BreadthFirst(vertex)
    DECLARE nodes <-- new List()
    DECLARE breadth <-- new Queue()
    breadth.Enqueue(vertex)

    while (breadth is not empty)
        DECLARE front <-- breadth.Dequeue()
        nodes.Add(front)

        for each child in front.Children
            if(child is not visited)
                child.Visited <-- true
                breadth.Enqueue(child)   

    return nodes;

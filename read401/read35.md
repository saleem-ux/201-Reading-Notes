## Graphs

A graph is a non-linear data structure that can be looked at as a collection of **vertices** (or **nodes**) potentially connected by line segments named **edges**.

### some common terminology used when working with Graphs:

1. **Vertex** - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
2. **Edge** - An edge is a connection between two nodes.
3. **Neighbor** - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
4. **Degree** - The degree of a vertex is the number of edges connected to that vertex.

-------------------------------------

### Directed vs Undirected

1. Undirected Graphs

- An **Undirected Graph** is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.

For example, in the graph below, Node **C** is connected to **Node A**, **Node E** and **Node B**. There are no “directions” given to point to specific vertices. The connection is bi-directional.

![undirectional](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/UndirectedGraph.PNG)

- The undirected graph we are looking at has 6 vertices and 7 undirected edges.
- Vertices/Nodes = {a,b,c,d,e,f}
- Edges = {(a,c),(a,d),(b,c),(b,f),(c,e),(d,e),(e,f)}

2. Directed Graphs (Digraph)

- A **Directed Graph** also called a **Digraph** is a graph where every edge is directed.
- Unlike an undirected graph, a **Digraph** has direction. Each node is directed at another node with a specific requirement of what node should be referenced next.

![directed](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/DirectedGraph.PNG)


- The directed graph above has six vertices and eight directed edges
- Vertices = {a,b,c,d,e,f}
- Edges = {(a,c),(b,c),(b,f),(c,e),(d,a),(d,e)(e,c)(e,f)}

---------------------------------

### Complete vs Connected vs Disconnected

1. Complete Graphs
A complete graph is when all nodes are connected to all other nodes.

2. Connected
A connected graph is graph that has all of vertices/nodes have at least one edge.

3. Disconnected
A disconnected graph is a graph where some vertices may not have edges.

------------------------

### Acyclic vs Cyclic

1. Acyclic Graph

- An acyclic graph is a directed graph without cycles.
- A cycle is when a node can be traversed through and potentially end up back at itself.

Here is an example of 3 acyclic graphs:

![acycle](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/threeAcyclic.png)

- A directed acyclic graph is also called a DAG. This can also be represented as what we know as a tree.


2. Cyclic Graphs

- A Cyclic graph is a graph that has cycles.
- A cycle is defined as a path of a positive length that starts and ends at the same vertex.

![cycle](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/cyclic.PNG)

--------------

[Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)

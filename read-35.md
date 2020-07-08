# Graphs
  -  is a non-linear data structure that can be looked at as a collection of `vertices` (or `nodes`) potentially connected by line segments named `edges`.

## common terminology:
  - 1. Vertex - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
  - 2. Edge - An edge is a connection between two nodes.
  - 3. Neighbor - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
  - 4. Degree - The degree of a vertex is the number of edges connected to that vertex.

## Directed vs Undirected 

  - **Undirected Graphs**
    - is a graph where each edge is undirected or bi-directional. This means that the undirected graph does not move in any direction.
  
  - **Directed Graphs (Digraph)**
    - is a graph where every edge is directed.

  - **Complete Graphs**
    - A complete graph is when all nodes are connected to all other nodes.

  - A `connected graph` is graph that has all of vertices/nodes have at least one edge.

  - A `disconnected graph` is a graph where some vertices may not have edges.

  - An `acyclic graph` is a directed graph without cycles.

  - A `cycle` is when a node can be traversed through and potentially end up back at itself.

  - An `adjacency list` is the most common way to represent graphs. An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.
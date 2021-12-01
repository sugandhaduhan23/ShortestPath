# ShortestPath
Shortest Path using Dijkstra and Bellman Ford Algorithm

**Shortest Path**

If we are searching for the shortest path from node X  to any other given node in the graph we need to look at all the possible paths from node X to node Y and pick the shortest.

The shortest path problem is about finding a path between 2 vertices in a graph such that the total sum of the edges weights is minimum.

The two most popular algorithm to find out the shortest path are :
1. Bellman Ford Algorithm
2. Dijkstra’s Algorithm

**Bellman Ford Algorithm**

1. The Bellman–Ford algorithm is an algorithm that computes shortest paths from a single source vertex to all of the other vertices in a weighted digraph.
2. It is slower than Dijkstra's algorithm for the same problem, but more versatile, as it is capable of handling graphs in which some of the edge weights are negative numbers.
3. Bellman Ford algorithm works by overestimating the length of the path from the starting vertex to all other vertices. Then it iteratively relaxes those estimates by finding new paths that are shorter than the previously overestimated paths.
This algorithm takes as input a directed weighted graph and a starting vertex. It produces all the shortest paths from the starting vertex to all other vertices.

**Dijkstra’s Algorithm**

Dijkstra's algorithm is an algorithm for finding the shortest paths between nodes in a graph.

1. Set the distance to the source to 0 and the distance to the remaining vertices to infinity. 
2. Set the current vertex to the source.
3. Flag the current vertex as visited.
4. For all vertices adjacent to the current vertex, set the distance from the source to the adjacent vertex equal to the minimum of its present distance and the sum of the weight of the edge from the current vertex to the adjacent vertex and the distance from the source to the current vertex.
5. From the set of unvisited vertices, arbitrarily set one as the new current vertex, provided that there exists an edge to it such that it is the minimum of all edges from a vertex in the set of visited vertices to a vertex in the set of unvisited vertices. To reiterate: The new current vertex must be unvisited and have a minimum weight edges from a visited vertex to it. This can be done trivially by looping through all visited vertices and all adjacent unvisited vertices to those visited vertices, keeping the vertex with the minimum weight edge connecting it. 
6. Repeat steps 3-5 until all vertices are flagged as visited.


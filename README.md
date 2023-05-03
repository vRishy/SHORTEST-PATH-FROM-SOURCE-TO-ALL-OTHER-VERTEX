# SHORTEST-PATH-FROM-SOURCE-TO-ALL-OTHER-VERTEX

The given problem involved finding the shortest path from a source vertex to all other
vertices in a graph. Two algorithmic techniques, Dijkstra’s algorithm and Bellman-Ford
algorithm were used to solve the problem. The graph as 9 vertices and 14 edges.
Dijkstra's algorithm works well when the graph has non-negative edge weights. It uses a
greedy approach and works in a top-down fashion. The algorithm maintains a priority queue
of vertices and repeatedly extracts the vertex with the minimum distance from the source. It
then updates the distances of all its neighbours. Dijkstra's algorithm has a time complexity of
O(E log V), where E is the number of edges and V is the number of vertices in the graph.
On the other hand, Bellman-Ford algorithm works well for graphs with negative edge
weights. It uses a bottom-up approach and works by relaxing all edges in the graph for V - 1
iterations, where V is the number of vertices in the graph. It then checks for negative cycles
in the graph, which can cause the algorithm to run indefinitely. Bellman-Ford algorithm has a
time complexity of O(VE), where E is the number of edges and V is the number of vertices in
the graph.

In the given problem, the graph did not have any negative edges, which made Dijkstra's
algorithm a better choice for solving the problem. The graph also did not have any negative
cycles, which made Bellman-Ford algorithm less suitable for the problem. Based on the time
complexity of the algorithms, Dijkstra's algorithm is more efficient for sparse graphs with
non-negative edge weights, while Bellman-Ford algorithm is more suitable for dense graphs
with negative edge weights. In conclusion, the algorithmic technique that worked well for the
given problem was Dijkstra's algorithm, which was able to find the shortest path from a
source vertex to all other vertices in the graph efficiently

In conclusion, both Dijkstra's algorithm and Bellman-Ford algorithm have their advantages
and disadvantages in solving the shortest path problem in a graph.
Dijkstra's algorithm is faster and more efficient than Bellman-Ford algorithm for graphs that
do not have negative edge weights. It has a time complexity of O(E log V) using a priority
queue data structure, making it suitable for large graphs. However, it cannot handle negative
edge weights, which limits its applicability.
On the other hand, Bellman-Ford algorithm can handle negative edge weights and can detect
negative cycles in a graph. It has a higher time complexity of O(V*E) compared to Dijkstra's
algorithm, making it slower for larger graphs. However, for small graphs with negative edge
weights or negative cycles, Bellman-Ford algorithm is the only viable option.
In the given problem, the graph did not have negative edge weights, making Dijkstra's
algorithm a suitable choice. The implementation of Dijkstra's algorithm produced the correct
shortest path distances in a faster time compared to Bellman-Ford algorithm. Therefore, in
this case, Dijkstra's algorithm worked well for the given problem.
However, if the problem had a graph with negative edge weights or negative cycles, BellmanFord algorithm would have been the better choice. In such cases, Dijkstra's algorithm would
have produced incorrect results or would not have been able to provide a solution at all.

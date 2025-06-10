##### Graphs
- A data structure representing connections among items
	- Computer networks
	- Product recommendations
	- Social Networks
- Are often used to represent a geographic map, which can contain information about places and travel routes
---
##### Graph Components
- Vertices (nodes)
- **Edges**
	- Connectedness
- Vertices in a graph can represent airports, with edges representing available flights
---
##### Terminology
- **Adjacent**
	- Two nodes are directly connected by an edge
- **Path** 
	- Sequence of edges leading from a source to a target
- **Path Length**
	- The total number of edges in a path
- *Distance*
	- The number of edges on the shortest path of two vertices
---
##### Other Terms
- **Edge Weights**
	- Associates a weight (cost, time, etc.) with each edge
	- often represents the length of a travel route, either in total distance or expected time
- **Directed Edges**
	- Sequence of directed edges leading from a source to a destination vertex
- **Cycle**
	- A path that starts and ends at the same vertex
	- A directed graph is cyclic if the graph contains a cycle, an acyclic if the graph does not contain a cycle
---
##### Adjacency Lists
- **Adjacency List** - In a n adjacency list graph representation, each vertex has a list of adjacent vertices, each list item representing an edge
---
##### Breadth First Search
- A **Breadth-First Search** traverses a graph by starting at a specific vertex and visiting the vertex's adjacent vertices before visiting the next closest vertices. No vertex is **re-visited**
---
##### Depth First Algorithm
- **Depth-First Search** traverses a graph by visiting a specific starting vertex, and then visiting every vertex along each path originating from the starting vertex. Each path is traversed to the path's end before **backtracking**.
	- Create a `vertexStack` and an empty `visitedSet`
	- Push starting node to `vertexStack`
	- `currentVertex = vertexStack.pop` add popped value to `visitedSet`
	- Check for adjacency of `currentVertex` add each to stack
	- Repeat until stack is empty
---
##### Dijkstra's Algorithm
- **Dijkstra's Algorithm** determines the shortest path from a start vertex to each vertex in a graph
- For each vertex, Dijkstra's algorithm determines the vertex's distance and predecessor pointer
	- **Distance is the shortest path distance from the start**
	- Vertex's **predecessor pointer** points to the previous vertex along the shortest pat
---
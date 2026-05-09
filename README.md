# **Serikbay Nurali** 
 # 🚀 Assignment 4 – Graph Traversal and Representation System

## 📚 Course Information

* **Course:** Data Structures and Algorithms
* **Assignment:** Assignment 4 – Graph Traversal and Representation System
* **Language:** Java
* **IDE:** IntelliJ IDEA

---

# 📖 Project Overview

This project implements a complete graph traversal system using Java.

The graph is represented using an **Adjacency List** structure and supports two major traversal algorithms:

* Breadth-First Search (BFS)
* Depth-First Search (DFS)

The system creates graphs of different sizes and analyzes traversal performance using execution time measurements.

---

# 🧩 Graph Structure

A graph consists of:

* **Vertices (Nodes)** → represent data points
* **Edges** → connections between vertices

Graphs are widely used in:

* Social Networks
* GPS Navigation
* Computer Networks
* Search Engines
* Path Finding Systems

---

# 📦 Project Structure

```text
assignment3-graphs/
├── src/
│   ├── Vertex.java
│   ├── Edge.java
│   ├── Graph.java
│   ├── Experiment.java
│   └── Main.java
├── docs/
│   ├── screenshots/
│   └── diagrams/
├── README.md
└── .gitignore
```

---

# 🏗️ Class Descriptions

## 🔹 Vertex Class

Represents a single node in the graph.

### Fields

* `id` → unique identifier

### Methods

* Constructor
* Getter
* `toString()`

### Example

```java
Vertex v = new Vertex(1);
```

---

## 🔹 Edge Class

Represents a connection between two vertices.

### Fields

* `source`
* `destination`

### Methods

* Constructor
* Getters
* `toString()`

### Example

```java
Edge edge = new Edge(v1, v2);
```

---

## 🔹 Graph Class

Stores the graph using an adjacency list.

### Adjacency List Example

```text
0 -> 1 2
1 -> 2 3
2 -> 3 4
```

### Advantages

✅ Memory Efficient
✅ Fast Traversal
✅ Easy Edge Management
✅ Suitable for Sparse Graphs

### Main Methods

```java
addVertex(Vertex v)
addEdge(int from, int to)
printGraph()
bfs(int start)
dfs(int start)
```

---

## 🔹 Experiment Class

Responsible for:

* Running BFS and DFS
* Measuring execution time
* Comparing performance results

### Time Measurement

```java
long start = System.nanoTime();
long end = System.nanoTime();
```

---

# 🔍 Breadth-First Search (BFS)

## 📌 Description

Breadth-First Search visits vertices level-by-level.

BFS explores all neighboring vertices before moving deeper into the graph.

---

## ⚙️ BFS Algorithm Steps

1. Start from source vertex
2. Mark vertex as visited
3. Add vertex into queue
4. Visit neighboring vertices
5. Repeat until queue becomes empty

---

## 📈 BFS Time Complexity

```text
O(V + E)
```

Where:

* `V` = Vertices
* `E` = Edges

---

## ✅ BFS Use Cases

* Shortest path search
* GPS systems
* Social networking
* Web crawling

---

# 🔍 Depth-First Search (DFS)

## 📌 Description

Depth-First Search explores deeply before backtracking.

DFS uses recursion or stack-based traversal.

---

## ⚙️ DFS Algorithm Steps

1. Start from source node
2. Mark node as visited
3. Visit neighbors recursively
4. Continue until all nodes are visited
5. Backtrack when necessary

---

## 📈 DFS Time Complexity

```text
O(V + E)
```

Where:

* `V` = Vertices
* `E` = Edges

---

## ✅ DFS Use Cases

* Cycle detection
* Maze solving
* Topological sorting
* Path finding

---

# 🧪 Experimental Results

## 📊 Execution Time Comparison

| Graph Size   | BFS Time (ns) | DFS Time (ns) |
| ------------ | ------------- | ------------- |
| 10 Vertices  | 1507500       | 405300        |
| 30 Vertices  | 775200        | 868400        |
| 100 Vertices | 2994200       | 2274600       |

---

# 📌 Observations

* Traversal time increased as graph size increased.
* DFS performed slightly faster in the experiments.
* Both algorithms showed approximately linear growth.
* Results matched the expected complexity:

```text
O(V + E)
```

---

# ❓ Analysis Questions

## 1️⃣ How does graph size affect BFS and DFS performance?

As the graph becomes larger, traversal time increases because more vertices and edges must be processed.

---

## 2️⃣ Which traversal was faster?

DFS was slightly faster in the experiments due to lower queue management overhead.

---

## 3️⃣ Do the results match expected complexity?

Yes.
The runtime growth followed the expected:

```text
O(V + E)
```

complexity.

---

## 4️⃣ How does graph structure affect traversal order?

* BFS explores level-by-level.
* DFS explores deeply before backtracking.

Different edge connections produce different traversal sequences.

---

## 5️⃣ When is BFS preferred?

BFS is preferred when:

* Finding shortest paths
* Searching nearest neighbors
* Working with unweighted graphs

---

## 6️⃣ What are DFS limitations?

* Large recursion stack usage
* Does not guarantee shortest path
* Can go very deep in large graphs

---

# 🖼️ Screenshots

<img width="1721" height="952" alt="image" src="https://github.com/user-attachments/assets/df5b7a16-d95f-4b1f-b3b0-d5e96d1be218" />
<img width="962" height="146" alt="image" src="https://github.com/user-attachments/assets/60efbedc-2804-424d-97bb-456d114cec14" />
<img width="411" height="132" alt="image" src="https://github.com/user-attachments/assets/6e17390b-cdb0-4837-8e17-d24ce48e206f" />




### Include:

* Graph structure output
* BFS traversal output
* DFS traversal output
* Performance comparison output

---

# 💭 Reflection

This assignment improved my understanding of graph traversal algorithms and graph representation using adjacency lists.

I learned the major differences between BFS and DFS and how both algorithms operate internally.

One challenge during implementation was managing visited vertices correctly to avoid infinite loops. Another challenge was implementing recursive DFS traversal efficiently.

Overall, this project strengthened my Java programming, problem-solving, and algorithm analysis skills.

---

# 🛠️ Technologies Used

* Java
* IntelliJ IDEA
* Git & GitHub

---

# 🔄 Git Commit History

```bash
git init

git add .
git commit -m "init: project structure"

git commit -m "feat(vertex): implemented Vertex class"

git commit -m "feat(edge): added Edge class"

git commit -m "feat(graph): implemented adjacency list"

git commit -m "feat(traversal): added BFS and DFS"

git commit -m "feat(experiment): added performance testing"

git commit -m "docs(readme): added project documentation"

git commit -m "release: v1.0"
```

---

# ✅ Conclusion

The project successfully implemented graph traversal and graph representation systems using Java.

Both BFS and DFS algorithms worked correctly for graphs of different sizes, and the experimental analysis confirmed the expected algorithm complexity.

This assignment demonstrated the practical importance of graph algorithms in computer science and real-world applications.

 




# 🏫 Campus Navigation and Utility Planner  
**Assignment 3 — Data Structures (ENCS205)**  
**Theme:** Trees and Graphs  

---

## 📘 Project Overview  
The **Campus Navigation and Utility Planner** is a Python-based software system designed to model a university campus using **trees** and **graph algorithms**.  
It helps visualize campus building relationships, find optimal paths, and plan resource layouts such as cables or pipelines efficiently.

This project demonstrates the implementation of:
- Binary Search Tree (BST)
- AVL Tree (Self-balancing tree)
- Graphs using Adjacency List & Matrix
- BFS and DFS traversals
- Dijkstra’s Algorithm (Shortest Path)
- Kruskal’s Algorithm (Minimum Spanning Tree)
- Expression Tree for energy bill calculations

---

## 🧩 Features Implemented
| Feature | Data Structure / Algorithm | Description |
|----------|----------------------------|--------------|
| Building Data Storage | Binary Search Tree | Stores campus building information |
| Self-Balancing Storage | AVL Tree | Ensures efficient insertions & searches |
| Campus Map | Graph (Adjacency List) | Represents paths between buildings |
| Traversals | BFS / DFS | Explores all campus connections |
| Optimal Path | Dijkstra’s Algorithm | Finds the shortest travel path |
| Utility Layout | Kruskal’s Algorithm | Plans minimal-cost cable layout |
| Expression Evaluation | Expression Tree | Calculates energy/utility costs |

---

## 🏗️ Project Structure
```
├── campus_navigation.py        # Main source code
├── Assignment3_Report_DS.docx  # Project report
├── README.md                   # Documentation (this file)
└── sample_output.txt           # Example output (optional)
```

---

## ⚙️ Setup & Execution

### Prerequisites
Make sure you have **Python 3.8+** installed.  
You can check by running:
```bash
python --version
```

### Clone Repository
```bash
git clone https://github.com/<your-username>/Campus-Navigation-Planner.git
cd Campus-Navigation-Planner
```

### Run Program
```bash
python campus_navigation.py
```

### Expected Output
```
=== Binary Search Tree ===
Inorder Traversal (BST): ['Admin', 'Library', 'CSE Dept', 'Hostel']

=== AVL Tree (with Rotations) ===
Inorder Traversal (AVL): ['Admin', 'Library', 'CSE Dept', 'Hostel']

=== Campus Graph ===
BFS from Library: ['Library', 'Admin', 'CSE Dept', 'Hostel']
DFS from Library: ['Library', 'Admin', 'Hostel', 'CSE Dept']
Shortest Paths (Dijkstra): {'Library': 0, 'Admin': 4, 'CSE Dept': 2, 'Hostel': 7}
Minimum Spanning Tree (Kruskal): [('Library', 'CSE Dept', 2), ('Library', 'Admin', 4), ('CSE Dept', 'Hostel', 5)]

=== Energy Bill Calculation ===
Result: 90.0
```

---

## 🧠 Data Structures Used

### 1. Binary Search Tree (BST)
- Inserts and searches building data based on `BuildingID`.
- Traversals: Inorder, Preorder, Postorder.

### 2. AVL Tree
- Automatically balances tree height using rotations.
- Demonstrates LL, RR, LR, RL rotations.

### 3. Graph
- Each building = Node  
- Each path = Edge with weight (distance)
- Represented using adjacency list.

### 4. Algorithms
| Algorithm | Purpose | Complexity |
|------------|----------|-------------|
| BFS | Level-order traversal | O(V + E) |
| DFS | Depth traversal | O(V + E) |
| Dijkstra | Shortest path | O((V + E) log V) |
| Kruskal | Minimum Spanning Tree | O(E log E) |

### 5. Expression Tree
- Evaluates postfix expressions like `10 20 + 3 * → 90`.

---

## 📈 Performance Analysis
| Component | Efficiency | Description |
|------------|-------------|--------------|
| BST | O(log n) | Fast retrieval but can be unbalanced |
| AVL Tree | O(log n) | Always balanced for efficient search |
| BFS/DFS | O(V + E) | Complete graph traversal |
| Dijkstra | O((V + E) log V) | Optimal routing |
| Kruskal | O(E log E) | Minimal-cost layout planning |

---

## 🏁 Conclusion
This project successfully demonstrates the use of **trees and graphs** in solving real-world problems like **campus navigation** and **utility layout planning**.  
It combines theoretical data structure concepts with practical implementation in Python for an efficient and scalable system.

---

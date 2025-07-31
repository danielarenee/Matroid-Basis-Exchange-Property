# Matroid Basis Exchange Property

This project implements an edge exchange algorithm between spanning trees of a graph — a concept rooted in matroid theory. Specifically, it illustrates the basis exchange property of the graphic matroid, where:

" Given two spanning trees 𝐴 and 𝐵, for any edge 𝑎 ∈ 𝐴∖𝐵, there exists an edge 𝑏 ∈ 𝐵∖𝐴 such that (𝐴 − {𝑎}) ∪ {𝑏} is also a spanning tree "

# What it Does 

* Builds a random Erdős–Rényi graph 𝐺(𝑛,𝑝)
* Generates two random spanning trees 𝐴 and 𝐵
* Computes the symmetric difference 𝐴∖𝐵, 𝐵∖𝐴
* Allows the user to pick an edge 𝑎 ∈ 𝐴∖𝐵
* Uses BFS to label components of 𝐴 − {𝑎}
* Identifies all 𝑏 ∈ 𝐵∖𝐴 that connect distinct components (valid exchanges)
* Allows the user to select a valid 𝑏, forming a new tree 𝐴′
* Visualizes: the original graph, trees 𝐴 and 𝐵, the edge difference sets and the final exchange operation with highlighted edges

# What I Learned

* Matroid Theory in Practice: Applied the basis exchange property of graphic matroids.
* Breadth-First Search (BFS): Used BFS to identify connected components after edge removal, enabling detection of valid replacement edges across components.
* Set Operations on Graph Edges
* Graph Visualization with NetworkX

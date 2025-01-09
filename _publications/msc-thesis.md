---
title: Disjoint Paths and Directed Steiner Tree on Planar Graphs with Terminals on Few Faces
link: https://studenttheses.uu.nl/handle/20.500.12932/42333
conf: Master&rsquo;s thesis
date: 2022-07-27

links:
    - name: Thesis presentation slides
      path: /assets/slides/msc-thesis-slides.pdf
      type: pdf
---
In the field of parameterized complexity, the main topic of interest is to make normally hard problems more tractable. A problem is in the complexity class FPT (fixed-parameter tractable) if it permits an algorithm with a running time bounded by $f(k) \cdot \text{poly}(n)$, where $n$ is the conventional input size and $k$ is some defined parameter of the input. The consequence of a problem being in FPT, is that it can be solved in polynomial time if the parameter is fixed, despite the problem being NP-hard generally. Many different parameters can be considered for fixed-parameter tractability: usually, this is a natural parameter arising from the problem formulation, such as the weight of a Steiner tree or the size of a dominating set, in their respective problems. Other parameters may be, for example, the output size, structural properties of an input graph (eg. treewidth).

A particularly interesting parameter is the *face cover number*, on problems whose input consists of a planar graph $G$ and a set of terminal vertices $K \subseteq V(G)$. The face cover number of such an input is then the minimum number of faces needed in a planar embedding of $G$, such that every terminal in $K$ is incident on at least one of those faces. While FPT graph problems already tend to perform better on planar graphs, this parameterization can create a further improvement for certain instances, where many terminals are incident on few faces.

Two problems are discussed in this thesis. Firstly, the Disjoint Paths problem is considered, which asks for a set of pairwise vertex-disjoint paths between given pairs of terminals in a graph. While it is a classically (very) hard problem, it has been shown to be fixed-parameter tractable. Different approaches to solving the problem are discussed, ending with a parameterization by the face cover number. The second considered problem is that of Directed Steiner Tree, which asks for a directed subtree of minimum weight in a graph, that connects all given terminals. The classic Dreyfus-Wagner algorithm for Steiner Tree is discussed, and it is shown that it can be modified for both the directed variant and one parameterized by the face cover number (and both). Next, a $2^{O(k)} \cdot n^{O(\sqrt{k})}$ algorithm by Kisfaludi-Bak et al. is explained, parameterized by the face cover number, and adapted to directed graphs.
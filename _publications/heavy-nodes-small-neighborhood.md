---
title: 'Heavy Nodes in a Small Neighborhood: Exact and Peeling  Algorithms with Applications'
link: https://ieeexplore.ieee.org/abstract/document/10792980
authors: [ling, hilde, huiping, greg, robert, leen, solon]
conf: IEEE Transactions on Knowledge and Data Engineering
date: 2024-12-11
---
We introduce a weighted and unconstrained variant of the well-known minimum $k$ union problem: Given a bipartite graph $\mathcal{G}(U,V,E)$ with weights for all nodes in $V$, find a set $S\subseteq V$ such that the ratio between the total weight of the nodes in $S$ and the number of their *distinct* adjacent nodes in $U$ is maximized.
Our problem, which we term *Heavy Nodes in a Small Neighborhood* (HNSN), finds applications in marketing, team formation, and money laundering detection.
For example, in the latter application, $S$ represents bank account holders who obtain illicit money from some peers of a criminal and route it through their accounts to a target account belonging to the criminal.
We prove that HNSN can be solved exactly in polynomial time via linear programming.
We also develop several algorithms offering different effectiveness/efficiency trade-offs: an exact algorithm, based on node contraction, graph decomposition, and linear programming, as well as three peeling algorithms.
The first peeling algorithm is a near-linear time approximation algorithm with a tight approximation ratio, the second is an iterative algorithm that converges to an optimal solution in a very small number of iterations in practice, and the third is a near-linear time greedy heuristic. In addition, we formalize a money laundering scenario involving multiple target accounts and show how our algorithms can be extended to deal with it. Our experiments on real and synthetic datasets show that our algorithms find (near-)optimal solutions, outperforming a natural baseline, and that they can detect money laundering more effectively and efficiently than two state-of-the-art methods.
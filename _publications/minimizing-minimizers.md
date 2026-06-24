---
title: Minimizing the Minimizers via Alphabet Reordering
link: https://www.sciencedirect.com/science/article/abs/pii/S030439752600191X
authors: [hilde, lorraine, greg, solon]
conf: Theoretical Computer Science, 115932
date: 2026-06-24

links:
    - name: CPM 2024 presentation slides
      path: /assets/slides/minimizing-minimizers-cpm.pdf
      type: pdf

citation: >
  Hilde Verbeek, Lorraine A.K. Ayad, Grigorios Loukides, and Solon P. Pissis. Minimizing the minimizers via alphabet reordering. Theoretical Computer Science, Volume 1076, 2026, 115932, https://doi.org/10.1016/j.tcs.2026.115932.

---

Minimizers sampling is one of the most widely-used mechanisms for sampling strings.
Let $S=S[1]\ldots S[n]$ be a string over a totally ordered alphabet $\Sigma$.
Further let $w\geq 2$ and $k\geq 1$ be two integers.
The minimizer of $S[i\ldots i+w+k-2]$ is the smallest position in $[i,i+w-1]$ where the lexicographically
smallest length-$k$ substring of $S[i\ldots i+w+k-2]$ starts.
The set of minimizers over all $i\in[1,n-w-k+2]$ is the set $\mathcal{M}_{w,k}(S)$ of the minimizers of $S$.

We consider the following basic problem: 

> Given $S$, $w$, and $k$, can we efficiently compute a total order on $\Sigma$ that minimizes $\|\mathcal{M}_{w,k}(S)\|$?


We show that this is unlikely by proving that the problem is NP-hard for any $w\geq 2$ and $k\geq 1$. Our result provides theoretical justification as to why there exist no exact algorithms for minimizing the minimizers samples, while there exists a plethora of heuristics for the same purpose. 
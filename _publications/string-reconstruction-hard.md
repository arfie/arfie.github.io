---
title: 'When is String Reconstruction using de Bruijn Graphs Hard?'
authors: [ben, sebastiaan, solon, leen, hilde]
link: https://dl.acm.org/doi/abs/10.1145/3841640
conf: Transactions on Algorithms, 2026
date: 2026-08-13

citation: >
  Ben Bals, Sebastiaan van Krieken, Solon Pissis, Leen Stougie, and Hilde Verbeek. 2025. When is String Reconstruction using de Bruijn Graphs Hard? In *European Symposium on Algorithms (ESA)*, 2025.
---

The reduction of the fragment assembly problem to (variations of) the classical Eulerian trail problem [Pevzner et al., PNAS 2001] has led to remarkable progress in genome assembly. This reduction employs the notion of *de Bruijn graph* $G=(V,E)$ of order $k$ over an alphabet $\Sigma$. A single Eulerian trail in $G$ represents a *candidate* genome reconstruction. Bernardini et al. have also introduced the complementary idea in data privacy [ALENEX 2020] based on $z$-anonymity. Let $S$ be a private string that we would like to release, preventing, however, its full reconstruction. For a privacy threshold $z>0$, we compute the largest $k$ for which there exist at least $z$ Eulerian trails in the order-$k$ de Bruijn graph of $S$, and release a string $S'$ obtained via a random Eulerian trail.

The pressing question is: How hard is it to reconstruct a best string from a de Bruijn graph given a function that models domain knowledge? Such a function maps every length-$k$ string to one *interval of positions* where it may occur in the reconstructed string. By the above reduction to de Bruijn graphs, the latter function translates into a function $c$ mapping every edge to an interval  where it may occur in an Eulerian trail. This gives rise to the following basic problem on graphs:

*Given an instance $(G,c)$, can we efficiently compute an Eulerian trail respecting $c$?*

Hannenhalli et al. [CABIOS 1996] formalized this problem and showed that it is NP-complete. Ben{-}Dor et al. [J. Comput. Biol. 2002] showed that it is NP-complete, even on de Bruin graphs with $\|\Sigma\|=4$. In this work, we settle the lower-bound side of this problem by showing that finding a $c$-respecting Eulerian trail in de Bruijn graphs over alphabets of size $2$ is NP-complete.

We then shift our focus to *parameterization* aiming to capture the quality of our domain knowledge in the complexity.
Ben{-}Dor et al. developed an algorithm to solve the problem on de Bruijn graphs in $O(m \cdot w^{1.5} 4^{w})$ time, where $m=|E|$ and $w$ is the *maximum interval length* over all edges in $E$. Bumpus and Meeks [Algorithmica 2023] later rediscovered the same algorithm on temporal graphs, which highlights the relevance of this problem in other contexts. Our central contribution is showing how combinatorial insights lead to *exponential-time* improvements over the state-of-the-art algorithm. In particular, for the important class of de Bruijn graphs, we develop an algorithm parametrized by $w (\log w+1) /(k-1)$: for a de Bruijn graph of order $k$, it runs in $O(mw \cdot 2^{\frac{w (\log w+1)}{k-1}})$ time. Our result improves on the state of the art by roughly an exponent of $(\log w +1)/(k-1)$. The existing algorithms have a natural interpretation for string reconstruction: when for each length-$k$ string, we know a small range of positions it must lie in, string reconstruction can be solved in linear time. Our improved algorithm shows that *it is enough when the range of positions is small relative to $k$*. 

We then generalize both the existing and our novel FPT algorithm by allowing the cost at every position of an interval to vary. In this optimization version, our hardness result translates into inapproximability and the FPT algorithms work with a slight extension. Surprisingly, even in this more general setting, we extend the FPT algorithms to count and enumerate the min-cost Eulerian trails. The counting result has direct applications in the data privacy framework of Bernardini et al.

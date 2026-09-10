---
title: 'Text Indexing: From Reporting to Counting'
authors: [ben, panos, oded, solon, hilde]
conf: European Symposium on Algorithms (ESA) 2026
date: 2026-7-1
link: https://arxiv.org/abs/2607.24043

citation: >
  tba
---

We prove an elementary yet powerful combinatorial lemma: in any rooted tree with $L$ leaves, the number of nodes whose depth is smaller than the number of their leaf descendants is at most $L$.
For any string $T$ of length $n$, a direct application of this lemma to the suffix trie of $T$ yields thatthe number of substrings of $T$ whose length is smaller than their number of occurrences in $T$ is at most $n$.
This combinatorial insight leads to space-efficient data structures with optimal query times for string _counting_ problems via the following algorithmic framework:
store the counts for the at most $n$ "frequent" substrings of $T$ in a preprocessing step, and use a _reporting_ query to count for the "infrequent" substrings.
Our framework acts as a convenient black box, lifting indexes with reporting time $O(|P|+|\text{Occ}_T(P)|)$ to support counting queries in time $O(|P|)$,
where $P$ is the queried pattern and $\text{Occ}_T(P)$ is the set of occurrences of $P$ in $T$.
As applications, we show efficient indexes for consecutive occurrences, weighted sequences, strings with utilities, and non-overlapping occurrences.

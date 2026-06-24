---
title: Faster Algorithms for Shortest Unique and Absent Substrings
link: https://arxiv.org/abs/2605.04826
authors: [panos, manal, solon, hilde, wiktor]
conf: Scandinavian Symposium on Algorithmic Theory (SWAT) 2026
date: 2026-5-6

citation: >
  Panagiotis Charalampopoulos, Manal Mohamed, Solon P. Pissis, Hilde Verbeek, and Wiktor Zuba. Faster Algorithms for Shortest Unique or Absent Substrings. In 20th Scandinavian Symposium on Algorithm Theory (SWAT 2026). Leibniz International Proceedings in Informatics (LIPIcs), Volume 370, pp. 13:1-13:19, Schloss Dagstuhl – Leibniz-Zentrum für Informatik (2026) https://doi.org/10.4230/LIPIcs.SWAT.2026.13
---

We revisit two well-known algorithmic problems on strings: computing a _shortest unique substring_ (SUS) and a _shortest absent substring_ (SAS) of a string $S$ of length $n$. Both problems admit folklore $O(n)$-time solutions using the suffix tree of $S$. However, for small alphabets, this complexity is not necessarily optimal in the word RAM model, where a string of length $n$ over alphabet $[0,\sigma)$ can be stored in $O(n \log \sigma/\log n)$ space and read in $O(n \log \sigma/\log n)$ time.

We present an $O(n \log \sigma/\sqrt{\log n})$-time algorithm for computing a SUS of $S$. This algorithm decomposes the problem according to the length and the period of the sought substring and uses several tools and techniques, such as synchronizing sets, the analysis of runs, and wavelet trees, to reduce the computation of a SUS to a simple geometric problem. Further, we adapt this algorithm and combine it with an efficient construction of de Bruijn sequences in order to obtain an $O(n \log \sigma/\sqrt{\log n})$-time algorithm for computing a SAS of $S$. 
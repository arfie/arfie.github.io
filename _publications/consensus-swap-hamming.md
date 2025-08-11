---
title: 'String Consensus Problems with Swaps and Substitutions'
authors: [esteban, laurent, gabriele, hilde]
link: https://arxiv.org/abs/2507.19139
conf: International Symposium on String Processing and Information Retrieval (SPIRE) 2025
date: 2025-07-28

citation: >
  Gabory, Estéban, et al. String Consensus Problems with Swaps and Substitutions. In *32nd International Symposium on String Processing and Information Retrieval (SPIRE)*, 2025.
---

String consensus problems aim at finding a string that minimizes some given distance with respect to an input set of strings. In particular, in the Closest string problem, we are given a set of strings of equal length and a radius $d$. The objective is to find a new string that differs from each input string by at most $d$ substitutions. We study a generalization of this problem where, in addition to substitutions, swaps of adjacent characters are also permitted, each operation incurring a unit cost. Amir et al. showed that this generalized problem is NP-hard, even when only swaps are allowed. In this paper, we show that it is FPT with respect to the parameter $d$. Moreover, we investigate a variant in which the goal is to minimize the sum of distances from the output string to all input strings. For this version, we present a polynomial-time algorithm. 
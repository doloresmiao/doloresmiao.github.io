---
title: "An Automated OpenMP Mutation Testing Framework for Performance Optimization"
collection: publications
category: manuscripts
permalink: /publication/2024-parco
excerpt: 'MUPPET is a source-level mutation testing framework for OpenMP programs that identifies and evaluates code changes to uncover performance defects and optimization opportunities overlooked by compiler IR-based methods, using multiple search algorithms to find mutations that yield speedups in 75.9% of tested benchmarks and proxy applications while preserving correctness.'
date: 2024-08-21
venue: 'Journal of Parallel Computing'
paperurl: 'http://doloresmiao.github.io/files/parco121.pdf'
bibtexurl: 'http://doloresmiao.github.io/files/parco121.tex'
citation: 'Dolores Miao, Ignacio Laguna, Giorgis Georgakoudis, Konstantinos Parasyris, Cindy Rubio-González, An automated OpenMP mutation testing framework for performance optimization, Parallel Computing, Volume 121, 2024, 103097, ISSN 0167-8191.'
---
Performance optimization continues to be a challenge in modern HPC software. Existing performance optimization techniques, including profiling-based and auto-tuning techniques, fail to indicate program modifications at the source level thus preventing their portability across compilers. This paper describes Muppet, a new approach that identifies program modifications called mutations aimed at improving program performance. Muppet’s mutations help developers reason about performance defects and missed opportunities to improve performance at the source code level. In contrast to compiler techniques that optimize code at intermediate representations (IR), Muppet uses the idea of source-level mutation testing to relax correctness constraints and automatically discover optimization opportunities that otherwise are not feasible using the IR. We demonstrate the Muppet’s concept in the OpenMP programming model. Muppet generates a list of OpenMP mutations that alter the program parallelism in various ways, and is capable of running a variety of optimization algorithms such as delta debugging, Bayesian Optimization and decision tree optimization to find a subset of mutations which, when applied to the original program, cause the most speedup while maintaining program correctness. When Muppet is evaluated against a diverse set of benchmark programs and proxy applications, it is capable of finding sets of mutations that induce speedup in 75.9% of the evaluated programs.

See the **code on GitHub**: [github.com/LLNL/MUPPET](https://github.com/LLNL/MUPPET)
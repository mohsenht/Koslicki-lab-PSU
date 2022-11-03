---
layout: paper_summary
title: "CMash: fast, multi-resolution estimation of k-mer-based Jaccard and containment indices"
---

### Summary
By storing and truncating k-mer sketches from the reference datasets in a ternary search tree, we can simultaneously obtain estimation of Jaccard index and containment index between reference data and arbitrary query data. With empirically negligible bias, we can obtain the estimation for a range of k values more efficiently.


### Abstract
K-mer based methods are used ubiquitously in the field of computational biology. However, determining the optimal value of k for a specific application often remains heuristic. Simply reconstructing a new k-mer set with another k-mer size is computationally expensive, especially in metagenomic analysis where data sets are large. Here, we introduce a hashing-based technique that leverages a kind of bottom-m sketch as well as a k-mer ternary search tree (KTST) to obtain k-mer based similarity estimates for a range of k values. By truncating k-mers stored in a pre-built KTST with a large k = kmax value, we can simultaneously obtain k-mer based estimates for all k values up to kmax. This truncation approach circumvents the reconstruction of new k-mer sets when changing k values, making analysis more time and space-efficient. For example, we show that when using a KTST to estimate the containment index between a RefSeq-based microbial reference database and simulated metagenome data for 10 values of k, the running time is close to 10x faster compared to a classic MinHash approach while using less than one-fifth the space to store the data structure. A python implementation of this method, CMash, is available at https://github.com/dkoslicki/CMash. The reproduction of all experiments presented herein can be accessed via https://github.com/KoslickiLab/CMASH-reproducibles.

<img src="../../images/publication/rxiv_CMash.png" />



---
layout: post
title: SCarborSNV
description: Single Cell DNA Variant Caller
image: assets/images/SCarborSNV.jpg
permalink: /projects/SCarborSNV
---

I joined a bioinformatics [research lab](https://yufeng-wu.uconn.edu/yufengs-group/){:target="\_blank"} at university and began studying genomics and their application to cancer. Specifically I studied algorithms for the emerging field of single cell whole genome DNA sequencing (scDNA-seq). While researching other variant calling algorithms for scDNA-seq, I realised that the ancestral relationship between single cells in a sample could potentially be leveraged to improve accuracy and efficiency by first reconstructing an evolutionary tree.

While working on this project I was to some extent "scooped" by the brilliant and elegant algorithm SCIΦ ([article in Nature Communications](https://www.nature.com/articles/s41467-018-07627-7){:target="\_blank"}) which uses Monte Carlo Markov models to explore the probability space of genetic trees. Nonetheless, I pressed on with my somewhat more rudimentary algorithm, which I turned into my undergraduate honours thesis.

SCarborSNV takes aligned, filtered sequence data and first uses [neighbour joining](https://en.wikipedia.org/wiki/Neighbor_joining){:target="\_blank"} to build a heuristic tree of cells. Next SCarborSNV infers a probability distribution of the position on the tree of each candidate mutation. Finally, this distribution over a tree is used as a prior for calling variants in each cell.

After designing the algorithm, I implemented it in C code and developed a robust CLI that would also work in a genomics "analysis pipeline" &mdash; including filtering, alignment and other programs to turn raw sequencing data into useful information. Its accuracy is similar to other scDNA-seq variant calling algorithms, and is asymptotically faster than the two most cutting edge algorithms of the time. When biologists start sequencing hundreds or thousands of single cells (currently studies look at tens) this will become much more important.

You can download and build the program [from GitHub](https://github.com/coldham10/SCarborSNV){:target="\_blank"}, and download the accompanying thesis [here](/assets/SCarborSNV.pdf){:target="\_blank"}.

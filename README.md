# AdvancedGenomics
It contains the project for the Advanced Genomics Course.
The 16S ribosomal RNA gene is the most widely used marker gene in microbial ecology. Counts of 16S sequence variants are used to estimate proportions of bacterial and archaeal taxa in microbial communities.
Because different organisms contain different 16S gene copy numbers (GCNs), sequence variant counts are biased towards clades with greater GCNs. Several tools have recently been developed for predicting GCNs using phylogenetic methods and based on sequenced genomes, in order to correct for this bias. 16S GCNs could only be accurately predicted for a limited fraction of taxa, namely taxa with closely to moderately related representatives (15% divergence in the 16S rRNA gene)
The idea is to implement a KNN algorithm for classification to predict the number of copies of 16S based on the similarity of 16S sequences of microorganisms with 16S sequences of microorganisms which have a known number of 16S copies. Before implementing the KNN classifier, it is necessary to cluster the data to see if sequences of the same species cluster together in the same cluster; otherwise it is not possible to implement an accurate 16S copy predictor.
Workflow
1) Data Retrieving
2) Data Cleaning
3) Visual inspection of the data
4) Computing the distance matrix using the Levensthein distance on raw sequences
5)Simple Hierarchical clustering
6) Analysis of the results using Entropy as a measure of cluster homogeneity
7) Hierarchical clustering with Genie module
8) Analysis of the results using Entropy as a measure of cluster homogeneity
9) KNN classifier using the Levensthein distance matrix and its evaluation
10) Kmers embedding and IDF representation of DNA sequences
11) KNN classifier on the IDF vectors varying the kmer length
12) Dimensionality reduction on IDF vectors
13) KNN classifier on the reduced space
14) Evaluation of all classifiers
15) Simple Hierarchical clustering on IDF vectors
16) Analysis of the results using Entropy as a measure of cluster homogeneity
17)Hierarchical clustering with the Genie module on IDF vectors
18) Analysis of the results using Entropy as a measure of cluster homogeneity

All data is retrieved from paper "Louca, S., Doebeli, M. & Parfrey, L.W. Correcting for 16S rRNA gene copy numbers in microbiome surveys remains an unsolved problem. Microbiome 6, 41 (2018). https://doi.org/10.1186/s40168-018-0420-9 '

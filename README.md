# CBP-JMF: An Improved Joint Matrix tri-Factorization Method for Characterizing Complex Biological Processes of Disease 

## Abstract

__Motivation:__ Matrix factorization techniques can integrative analysis multi-dimensional genomic data across the same samples. We present CBP-JMF, a framework for discovering complex biological processes (CBPs) that underlying sample groups. Different from existing methods, CBP-JMF is based on a de novo semi-supervised matrix tri-factorization that take labeled samples as prior information, classify the unlabeled samples, and devote to identify the underlying CBPs of groups. 

__Methods:__ CBP-JMF factorization decomposes several **non-negative matrix X<sub>i</sub>** into three matrices: **Molecular Coefficient Matrix U<sub>i</sub>**, **Factor Absorbing W<sub>i</sub>**, **Sample Basis Matrix V**. We use euclidean distance as cost function(so it's an optimization problem) to measure the distance between X<sub>i</sub>  and reconstructed  U<sub>i</sub>W<sub>i</sub>V. Besides, we incorporate samples’ label information into NMF through a graph embedding constraint and we give different input X<sub>i</sub> a unique weight to donate its contribution in optimization. Given input matrices  X<sub>i</sub> , labeled samples' subgroup and a correlation matrix of labeled samples, CBP-JMF integrate MG data (e.g., copy number variation, gene expression, microRNA expression, and/or gene network) to classify the unlabeled samples into groups and identify the underlying CBPs which characterize functional properties of each group.

__Results:__ We evaluate CBP-JMF on breast cancer, classify unlabeled samples into four subtypes (Lumina A, Luminal B, Basal like, Her2) and  highlight characteristic heterogeneous molecular pathways driving subtypes.  
​    

## The package

* CBP_JMF.py	This software package contains all the functions of CBP-JMF.Users can use command line 'pip install CBP_JMF' to install or download CBP_JMF.py and import it.  
* [__pypi.org__](https://pypi.org/project/CBP-JMF/#files) Our Package can also be downloaded here.
## Analysis scripts

* BRCA_example.ipynb	Run the CBP_JMF package on BRCA's mRNA data and miRNA data.   
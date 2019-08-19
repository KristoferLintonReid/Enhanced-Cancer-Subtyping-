# Enhanced-Cancer-Subtyping-
Enhanced Cancer Subtyping MRes Project Imperial College London 

## Abstract 

### Introduction

Subtyping of tumor transcriptome expression profiles is a routine method used to distinguish tumor heterogeneity. Unsupervised clustering techniques are often combined with survival analysis to decipher the relationship between genes and the survival times of patients. However, the reproducibility of these subtyping based studies is poor. There are multiple reports which have conflicting subtype and gene-survival time relationship results. 

In this study, the issues underlying the lack of reproducibility in transcriptomic subtyping studies were intordiuced. This problem arises from the routine analysis of small cohorts (< 100 individuals) and use of biased traditional consensus clustering techniques. This approach carefully combines multiple RNA-sequencing and microarray datasets, followed by subtyping via Monte-Carlo Consensus Clustering and creation of deep subtyping classifiers. This paper demonstrated an improved subtyping methodology, by investigating pancreatic ductal adenocarcinoma. 

This new approach also enables a degree of reproducibility, via the depl leareneining pancreatic ductal adenocarcinoma classifier, PDACNet, which classical subtyping studies have failed to establish.

Importantly, the methodology displayed identifies six biologically novel pancreatic ductal adenocarcinoma subtypes.

### Methods 

As part of this project, the largest open source transcriptomic pancreatic
ductal adenocarcinoma dataset was created by combining11 publicly available
PDAC Microarray datasets, and 3 RNA-sequencing datasets derived from solid tumor biopsies (Support Information Table 1).

The subtyping approach encompasses 4 key components:
1)Clustering with Monti-Carlo-Consensus-Clustering
2) Biological validation via Kaplan-Meier
survival analysis
3) Differential Expression
4) Subtype Classifier Creation


### Results 

#### M3C Clustering Analysis Indicates prior NMF results (Bailey et al., (2016) and Collinson et al., (2015), have identified false possitives.

![Monti-Carlo_Clustering_Bailey_etl al.,](https://github.com/KristoferLintonReid/Enhanced-Cancer-Subtyping-/blob/master/Images/Bailey_M3C.png)

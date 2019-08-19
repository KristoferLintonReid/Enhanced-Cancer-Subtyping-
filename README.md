# Enhanced-Cancer-Subtyping-
Enhanced Cancer Subtyping MRes Project Imperial College London  

## Introduction

Subtyping of tumor transcriptome expression profiles is a routine method used to distinguish tumor heterogeneity. Unsupervised clustering techniques are often combined with survival analysis to decipher the relationship between genes and the survival times of patients. However, the reproducibility of these subtyping based studies is poor. There are multiple reports which have conflicting subtype and gene-survival time relationship results. 

In this study, the issues underlying the lack of reproducibility in transcriptomic subtyping studies were intordiuced. This problem arises from the routine analysis of small cohorts (< 100 individuals) and use of biased traditional consensus clustering techniques. This approach carefully combines multiple RNA-sequencing and microarray datasets, followed by subtyping via Monte-Carlo Consensus Clustering and creation of deep subtyping classifiers. This paper demonstrated an improved subtyping methodology, by investigating pancreatic ductal adenocarcinoma. 

This new approach also enables a degree of reproducibility, via the depl leareneining pancreatic ductal adenocarcinoma classifier, PDACNet, which classical subtyping studies have failed to establish.

Importantly, the methodology displayed identifies six biologically novel pancreatic ductal adenocarcinoma subtypes.

## Methods 

#### *As part of this project, the largest open source transcriptomic pancreatic ductal adenocarcinoma dataset was created by combining 11 publicly available PDAC Microarray datasets, and 3 RNA-sequencing datasets derived from solid tumor biopsies (Support Information Table 1).*

** Table 1: original opensource data sets Combined to create a large PDAC cohort (1013 samples). ** 

![All 14 Original Cohort Sources ](https://github.com/KristoferLintonReid/Enhanced-Cancer-Subtyping-/blob/master/Images/Original-opensource_PDAC_Cohorts.png)


The subtyping approach encompasses 4 key components:
1)Clustering with Monti-Carlo-Consensus-Clustering
2) Biological validation via Kaplan-Meier
survival analysis
3) Differential Expression
4) Subtype Classifier Creation


## Results 

### **Monte-Carlo Consenss Clustering (M3C)**
#### *M3C Clustering Analysis Indicates prior NMF results (Bailey et al., (2016), have identified false possitives. Similarly with Collinson et al., (Collinson Results Avaliable at Enhnaced-Canacer-Subyping/Images/)* 

 **Figure 1 M3C Bailey et al., (2016)** 

![Monti-Carlo_Clustering_Bailey_etl al.,](https://github.com/KristoferLintonReid/Enhanced-Cancer-Subtyping-/blob/master/Images/Bailey_M3C.png)
 
 #### *M3C Clusterng Analyisis identifies 6 Subtypes of the 1013 Patient Cohort* 
 
  **Figure 2 M3C 1013 PDAC patient Cohort** ![Monti-Carlo_Clustering_of_1013 Patient Cohort identifies 6 Subypes.,](https://github.com/KristoferLintonReid/Enhanced-Cancer-Subtyping-/blob/master/Images/M3C_1013_PDAC-Cohort.png)
 
 
### **Biological and Clinical Validation** 


**Figure 3 A) Consensus matrix Heatmap, B) Heatmap of 2000 most variable genes against subtypes (Full list of DE genes inEhnaced-Cancer-Subtyping/Data/) , C) PCA Score plot of subtypes, D) Kaplan-Meier Survival Analyis** 
![Clincal nd biological validation of the 6 subtypes ](https://github.com/KristoferLintonReid/Enhanced-Cancer-Subtyping-/blob/master/Images/Biological%20and%20Clincal%20Validation.png)


### **Subtype Classifier Creation** 

#### *A deep learning subtype classifeier was created using the pakacge h20 and the autML function. this created 100  different ML based classifiers.* 

**Table 2 Top 5 Classifiers in terms of mean per class error, the top classififer was selected as PDACNet.**

![Top 5 Classifiers Created by H2O's AutoM gunction](https://github.com/KristoferLintonReid/Enhanced-Cancer-Subtyping-/blob/master/Images/h2O_ML_Top5_Classifiers.png)

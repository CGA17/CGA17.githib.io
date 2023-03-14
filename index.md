---
layout: default
title: "Comparing the Effects of Increased Sequencing Coverage on Analyses of Human Genetic Variation"
doodle: "/Double-helix.png"

---

Group A17: Karthik Guruvayurappan, Michael Nodini, Maddie LaScola, Andrew Li

---
* TOC
{:toc}
---

<details>
  <summary>Some Helpful Introduction Info!</summary>
  
  ### GWAS
  
  ### Genetic Diseases
  
  ### eQTL - Expression Quantitative Trait Loci 
</details>
  
## Introduction

### GWAS
Genome wide association studies (GWAS) are a way for scientists to identify inherited genetic variants associated with risk of disease for a particular trait. This method studies the entire set of DNA, also known as a genome, from a population searching for small variations called single nucleotide polymorphisms also known as SNPs. These small variations can lead to an increased chance of developing diseases later in life such as lung cancer. Variations in genetic expression lead to altered production of proteins which alter the functions of cells inside the body.
  
### Genetic Diseases
These small variations are responsible for changes as small as hair color up to life altering diseases. For example, sickle cell anemia stems from a mutation on a gene responsible for encoding the hemoglobin molecule on red blood cells. Due to the mutation, the red blood cells are formed in a sickle shape rather than round and can block blood flow leading to discomfort along with other afflictions. If these risks are discovered early on in one’s life preventative measures can be taken to decrease the likelihood of developing the disease or additional screenings can be scheduled to monitor an individual and catch the disease before it causes untreatable damage. Understanding how genetic expression translates to the observable traits we express is a necessary step towards providing insights for disease treatment, risk, prevention, and heritability.
  
### eQTL - Expression Quantitative Trait Loci
Expression quantitative trait loci (eQTLs) are SNPs associated with gene expression. However, linear models used in previous studies to identify eQTLs have been confounded by linkage disequilibrium (LD), making it difficult to determine causal relationships. Fine-mapping, which determines high-confidence SNPs likely to include causal variants, can be used to improve eQTL identification. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq, can reveal cell-type specific eQTL strength and underlying biological pathways. Recent advances in the 1000 Genomes Project have resulted in a high-coverage whole-genome sequencing dataset for the 1000 Genomes Project cohort, which could lead to improved eQTL identification and better location of causal SNPs.


## Abstract

Genome-wide association studies aim to find associations between single nucleotide polymorphisms (SNPs) at individual genomic positions and phenotypes like height or diabetes. Expression quantitative trait loci (eQTLs) are SNPs that are significantly associated with the expression of a certain gene. However, the link between genetic variation and observable phenotypes is still not fully understood, and eQTL analyses help to bridge this gap by linking genetic variation to gene expression that informs downstream phenotypes. To refine these associations, downstream analyses such as fine-mapping and functional annotation enrichment can be used to locate causal variants across the genome. Nevertheless, coverage, which is the average number of times each nucleotide is sequenced, is crucial to the power of SNP detection. In this study, we combine eQTL analyses with both fine-mapping and functional annotation enrichment to compare a low-coverage and a high-coverage dataset from a cohort in the 1000 Genomes Project.

<img align="center" width="1000" height="250" src = "/LHCoverage.png">


### Datasets

The analysis requires specific genome data from the 1000 Genomes Project and the European Nucleotide Archive, including newer data from the 1000 Genomes Project for genome assembly, and data under project names PRJEB31736 and PRJEB36890 from the European Nucleotide Archive. Results will be communicated in a research paper detailing the methods and software used, including tables and figures showcasing findings. The paper will focus on comparing two genome assemblies and discussing whether the new approach has improved eQTL results and identified more causal SNPs.

## Background
Genome-wide association studies (GWAS) identify genetic variants linked to phenotypes, such as disease, risk, or height. Expression quantitative trait loci (eQTLs) are genetic variants associated with gene expression, but their associations are confounded by linkage disequilibrium (LD). Fine-mapping methods are used to pinpoint causal variants. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq, determines eQTL function. The 1000 Genomes Project now provides higher sequencing coverage datasets, enabling more advanced analyses.


## Results

This section contains figures we've produced highlighing differences between the 2 analyses: higher/lower coverage.

<img align="center" width="650" height="400" src = "/Fig1.png"> <br />
### Figure 1

QQ-plots of eQTLs on Chromosome 22 for low coverage and high coverage genotyping. The low coverage (left) had a total of 1,802,930 association tests to identify 4,035 significant cis-eQTLs, while the high coverage had 2,151,453 association tests to identify 4,321 significant cis-eQTLs. (p-value < 5e-8) 


<img align="center" width="700" height="400" src = "/assets/img/fig3.jpg"> <br />
### Figure 2

P-value plots for association tests between SNPs proximal to the FAM118A gene and FAM118A RNA-seq expression. 


<img align="center" width="700" height="400" src = "/assets/img/fig2.jpg"> <br />
### Figure 3

Fine-mapped posterior inclusion probabilities for SNPs proximal to the FAM118A gene and FAM118A gene expression. Blue dots indicate credible sets for potential causal SNPs. There were 3 candidate SNPs in the low coverage data, and 35 candidate SNPs in the high coverage data.


## Methods
Datasets were obtained from the 1000 Genomes Project aligned to GRCh38
Raw VCF (variant call file) processing was performed using the plink package
Gene annotations were converted from GRCh37 to GRCh38 using UCSC LiftOver (http://genome.ucsc.edu)
eQTL calling was performed using the Matrix eQTL R package ⁹ The eQTL calling follows a linear regression.
eQTL Regression Equation: Y = XB + e
Fine-mapping was performed using the susieR R package1


## Conclusions

- Higher coverage sequencing data for genotyping identifies a greater number of eQTLs
- When finemapping eQTLs, higher coverage sequencing data identifies a larger number of potential causal SNPs (overlap with GTEx whole blood eQTLs)12
- Results are potentially confounded by population structure

<img align="right" width="300" height="350" src = "/Double-helix.png">
## References

1. [Lappalainen, Nature (2013)](https://doi.org/10.1038/nature12531)
2. [Pritchard, American Journal of Human Genetics (2001)](https://pubmed.ncbi.nlm.nih.gov/11410837/)
3. [Hormozdiari, Genetics (2014)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4196608/)
4. [Amariuta, American Journal of Human Genetics (2019)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6506796/)
5. [Buenrostro, Current Protocols in Molecular Biology (2015)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC4374986/)
6. [Subramanian, Proceedings of the National Academy of Sciences (2005)](https://www.pnas.org/doi/10.1073/pnas.0506580102) 
7. [Byrska-Bishop, Cell (2022)](https://pubmed.ncbi.nlm.nih.gov/36055201/)
8. [Purcell, American Journal of Human Genetics (2007)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1950838/) 
9. [Shabalin, Bioinformatics (2012)](https://www.researchgate.net/publication/223974050_Matrix_eQTL_Ultra_fast_eQTL_analysis_via_large_matrix_operations)
10. [Kundaje, Nature (2015)](https://doi.org/10.1038/nature14248)

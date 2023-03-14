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

<img align="right" width="200" height="300" src = "/Double-helix.png">
<details>
  <summary>Some Helpful Introduction Info!</summary>
  <p>
  ## GWAS
  
  ## Genetic Diseases
  
  ## eQTL - Expression Quantitative Trait Loci 
  </p>
</details>
  
  
### GWAS
Genome wide association studies (GWAS) are a way for scientists to identify inherited genetic variants associated with risk of disease for a particular trait. This method studies the entire set of DNA, also known as a genome, from a population searching for small variations called single nucleotide polymorphisms also known as SNPs. These small variations can lead to an increased chance of developing diseases later in life such as lung cancer. Variations in genetic expression lead to altered production of proteins which alter the functions of cells inside the body.
  
### Genetic Diseases
These small variations are responsible for changes as small as hair color up to life altering diseases. For example, sickle cell anemia stems from a mutation on a gene responsible for encoding the hemoglobin molecule on red blood cells. Due to the mutation, the red blood cells are formed in a sickle shape rather than round and can block blood flow leading to discomfort along with other afflictions. If these risks are discovered early on in one’s life preventative measures can be taken to decrease the likelihood of developing the disease or additional screenings can be scheduled to monitor an individual and catch the disease before it causes untreatable damage. Understanding how genetic expression translates to the observable traits we express is a necessary step towards providing insights for disease treatment, risk, prevention, and heritability.
  
### eQTL - Expression Quantitative Trait Loci
Expression quantitative trait loci (eQTLs) are SNPs associated with gene expression. However, linear models used in previous studies to identify eQTLs have been confounded by linkage disequilibrium (LD), making it difficult to determine causal relationships. Fine-mapping, which determines high-confidence SNPs likely to include causal variants, can be used to improve eQTL identification. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq, can reveal cell-type specific eQTL strength and underlying biological pathways. Recent advances in the 1000 Genomes Project have resulted in a high-coverage whole-genome sequencing dataset for the 1000 Genomes Project cohort, which could lead to improved eQTL identification and better location of causal SNPs.


## Abstract

Genome-wide association studies aim to find associations between single nucleotide polymorphisms (SNPs) at individual genomic positions and phenotypes like height or diabetes. Expression quantitative trait loci (eQTLs) are SNPs that are significantly associated with the expression of a certain gene. However, the link between genetic variation and observable phenotypes is still not fully understood, and eQTL analyses help to bridge this gap by linking genetic variation to gene expression that informs downstream phenotypes. To refine these associations, downstream analyses such as fine-mapping and functional annotation enrichment can be used to locate causal variants across the genome. Nevertheless, coverage, which is the average number of times each nucleotide is sequenced, is crucial to the power of SNP detection. In this study, we combine eQTL analyses with both fine-mapping and functional annotation enrichment to compare a low-coverage and a high-coverage dataset from a cohort in the 1000 Genomes Project.

<img align="center" width="900" height="250" src = "/LHCoverage.png">


### Datasets

The analysis requires specific genome data from the 1000 Genomes Project and the European Nucleotide Archive, including newer data from the 1000 Genomes Project for genome assembly, and data under project names PRJEB31736 and PRJEB36890 from the European Nucleotide Archive. Results will be communicated in a research paper detailing the methods and software used, including tables and figures showcasing findings. The paper will focus on comparing two genome assemblies and discussing whether the new approach has improved eQTL results and identified more causal SNPs.

## Background
Genome-wide association studies (GWAS) identify genetic variants linked to phenotypes, such as disease, risk, or height. Expression quantitative trait loci (eQTLs) are genetic variants associated with gene expression, but their associations are confounded by linkage disequilibrium (LD). Fine-mapping methods are used to pinpoint causal variants. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq, determines eQTL function. The 1000 Genomes Project now provides higher sequencing coverage datasets, enabling more advanced analyses.


## Results

This will contain figures we've produced highlighing differences between the 2 analyses: higher/lower coverage.

<img align="center" width="650" height="400" src = "/Fig1.png"> <br />
Figure 1

<img align="center" width="700" height="400" src = "/assets/img/fig3.jpg"> <br />
Figure 2

<img align="center" width="700" height="400" src = "/assets/img/fig2.jpg"> <br />
Figure 3

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


## References

1. Lappalainen, Nature (2013) 
2. Pritchard, American Journal of Human Genetics (2001) 
3. Hormozdiari, Genetics (2014) 
4. Amariuta, American Journal of Human Genetics (2019) 
5. Buenrostro, Current Protocols in Molecular Biology (2015) 
6. Subramanian, Proceedings of the National Academy of Sciences (2005) 
7. Byrska-Bishop, Cell (2022) 
8. Purcell, American Journal of Human Genetics (2007) 
9. Shabalin, Bioinformatics (2012) 
10. Kundaje, Nature (2015)

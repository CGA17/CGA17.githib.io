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
<img align="right" width="100" height="100" src = "/Double-helix.png">

## Introduction
Genome-wide association studies (GWAS) search for small variations or single nucleotide polymorphisms (SNPs) in the DNA of a population, which can increase the risk of developing diseases later in life, such as lung cancer. These variations affect genetic expression, leading to changes in protein production and altered cell function. Genetic mutations can cause minor changes such as hair color or severe diseases such as sickle cell anemia, which results from a mutation in the hemoglobin gene. Early detection of these genetic risks can lead to preventative measures or monitoring to catch the disease early. GWAS can provide insights into disease treatment, risk, prevention, and heritability by understanding the relationship between genetic expression and observable traits.

Expression quantitative trait loci (eQTLs) are genetic variants that are associated with gene expression. However, eQTL mapping using linear models can be confounded by linkage disequilibrium (LD), and further methods development is required to determine the functional significance of eQTLs. Fine-mapping can help identify high-confidence SNPs that include causal variants. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq, can reveal cell-type specific eQTL strength and underlying biological pathways. The recent advances in genome assembly by the Telomere-to-Telomere (T2T) consortium have resulted in a complete human genome assembly, which could improve eQTL mapping and identification of causal SNPs by reanalyzing eQTLs using this improved genome assembly.

The analysis requires specific genome data from the 1000 Genomes Project and the European Nucleotide Archive, including newer data from the 1000 Genomes Project for genome assembly, and data under project names PRJEB31736 and PRJEB36890 from the European Nucleotide Archive. Results will be communicated in a research paper detailing the methods and software used, including tables and figures showcasing findings. The paper will focus on comparing two genome assemblies and discussing whether the new approach has improved eQTL results and identified more causal SNPs.



## Background
Genome-wide association studies (GWAS) identify genetic variants linked to phenotypes, such as disease risk or height. Expression quantitative trait loci (eQTLs) are genetic variants associated with gene expression, but their associations are confounded by linkage disequilibrium (LD). Fine-mapping methods are used to pinpoint causal variants. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq, determines eQTL function. The 1000 Genomes Project now provides higher sequencing coverage datasets, enabling more advanced analyses.


## Abstract

Genome-wide association studies link individual genetic variants called single nucleotide polymorphisms (SNPs) with observable phenotypes. Expression quantitative trait loci (eQTLs) are SNPs associated with gene expression, providing insight into how genetic variation affects phenotypes. To better understand this link, eQTL analyses can be refined using fine-mapping and functional annotation enrichment. However, the power to detect SNPs depends on sequencing coverage. This analysis compares a high-coverage and low-coverage dataset from the 1000 Genomes Project, using eQTL analyses, fine-mapping, and functional annotation enrichment to better locate causal variants.


## Results

This will contain figures we've produced highlighing differences between the 2 analyses: higher/lower coverage.

## Methods
Raw VCF (variant call file) processing was performed using the plink package.⁸
eQTL calling was performed using the Matrix eQTL R package ⁹ The eQTL calling follows a linear regression.
Fine-mapping for causal variants was performed using the CAVIAR package.³
ATAC-seq data was obtained from the Roadmap Epigenomics Consortium.¹⁰
Gene set enrichment analysis was performed using the GSEA software.⁶
Datasets were obtained from the 1000 Genomes Project aligned to GRCh38.⁷


## Conclusions

INSERT CONCLUSIONS HERE (IDEALLY BETTER COVERAGE = BETTER  RESULTS)

## References

1. Lappalainen, Nature (2013) 2. Pritchard, American Journal of Human Genetics (2001) 3. Hormozdiari, Genetics (2014) 4. Amariuta, American Journal of Human Genetics (2019) 5. Buenrostro, Current Protocols in Molecular Biology (2015) 6. Subramanian, Proceedings of the National Academy of Sciences (2005) 7. Byrska-Bishop, Cell (2022) 8. Purcell, American Journal of Human Genetics (2007) 9. Shabalin, Bioinformatics (2012) 10. Kundaje, Nature (2015)

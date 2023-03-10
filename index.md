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
Genome-wide association studies (GWAS) help identify genetic variants linked to disease risk for a particular trait by analyzing the entire DNA (genome) from a population for small variations known as single nucleotide polymorphisms (SNPs). Variations in genetic expression due to these small variations can lead to changes as minor as hair color or as major as life-altering diseases like lung cancer or sickle cell anemia. By discovering these risks early, preventive measures can be taken or screenings scheduled to catch the disease before it becomes untreatable. Understanding how genetic expression affects observable traits is critical to gain insights into disease treatment, risk, prevention, and heritability.

Expression quantitative trait loci (eQTLs) are SNPs associated with gene expression. However, linear models used in previous studies to identify eQTLs have been confounded by linkage disequilibrium (LD), making it difficult to determine causal relationships. Fine-mapping, which determines high-confidence SNPs likely to include causal variants, can be used to improve eQTL identification. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq, can reveal cell-type specific eQTL strength and underlying biological pathways. Recent advances in the 1000 Genomes Project have resulted in a high-coverage whole-genome sequencing dataset for the 1000 Genomes Project cohort, which could lead to improved eQTL identification and better location of causal SNPs.

The analysis requires specific genome data from the 1000 Genomes Project and the European Nucleotide Archive, including newer data from the 1000 Genomes Project for genome assembly, and data under project names PRJEB31736 and PRJEB36890 from the European Nucleotide Archive. Results will be communicated in a research paper detailing the methods and software used, including tables and figures showcasing findings. The paper will focus on comparing two genome assemblies and discussing whether the new approach has improved eQTL results and identified more causal SNPs.

## Background
Genome-wide association studies (GWAS) identify genetic variants linked to phenotypes, such as disease, risk, or height. Expression quantitative trait loci (eQTLs) are genetic variants associated with gene expression, but their associations are confounded by linkage disequilibrium (LD). Fine-mapping methods are used to pinpoint causal variants. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq, determines eQTL function. The 1000 Genomes Project now provides higher sequencing coverage datasets, enabling more advanced analyses.


## Abstract

Genome-wide association studies link genetic variation to observable traits such as disease risk. eQTLs are SNPs that are significantly associated with gene expression, allowing researchers to better understand the link between genetic variation and downstream phenotypes. Refining these associations with fine-mapping and functional annotation enrichment can locate causal variants across the genome. However, coverage is important for detecting SNPs. In this study, researchers compare a high-coverage and low-coverage dataset from a cohort in the 1000 Genomes Project using eQTL analysis with fine-mapping and functional annotation enrichment.


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

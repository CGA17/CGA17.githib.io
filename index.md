---
layout: pages
title: "Group A17"
nav_exclude: true
---

# Comparing the Effects of Increased Sequencing Coverage on Analyses of Human Genetic Variation

Group A17: Karthik Guruvayurappan, Michael Nodini, Maddie LaScola, Andrew Li

## Introduction 
The Introduction Will Go Here

## Background
### Genome wide association studies (GWAS) allow for scientists to identify genetic variants associated with phenotypes like height or disease risk.
### Expression quantitative trait loci (eQTLs) are genetic variants that are significantly associated with gene expression.1
### eQTL associations are confounded by linkage disequilibrium (LD), where individual DNA positions are not inherited independently.
### Fine-mapping uses further statistical methods to pinpoint potential causal variants
### Quantifying eQTL enrichment with functional annotations, such as ATAC-seq for accessible chromatin, provides a mechanism for determining eQTL function.4,5
### Recent advances in the 1000 Genomes Project now provide higher sequencing coverage datasets.7

## Abstract

## Results

This will contain figures we've produced highlighing differences between the 2 analyses: higher/lower coverage.

## Methods
### Raw VCF (variant call file) processing was performed using the plink package.⁸
### eQTL calling was performed using the Matrix eQTL R package ⁹ The eQTL calling follows a linear regression.
### Fine-mapping for causal variants was performed using the CAVIAR package.³
### ATAC-seq data was obtained from the Roadmap Epigenomics Consortium.¹⁰ 
### Gene set enrichment analysis was performed using the GSEA software.⁶ 
### Datasets were obtained from the 1000 Genomes Project aligned to GRCh38.⁷


## Conclusions

### INSERT CONCLUSIONS HERE (IDEALLY BETTER COVERAGE = BETTER  RESULTS)

## References

### 1. Lappalainen, Nature (2013) 2. Pritchard, American Journal of Human Genetics (2001) 3. Hormozdiari, Genetics (2014) 4. Amariuta, American Journal of Human Genetics (2019) 5. Buenrostro, Current Protocols in Molecular Biology (2015) 6. Subramanian, Proceedings of the National Academy of Sciences (2005) 7. Byrska-Bishop, Cell (2022) 8. Purcell, American Journal of Human Genetics (2007) 9. Shabalin, Bioinformatics (2012) 10. Kundaje, Nature (2015)


---
layout: default
title: "Comparing the Effects of Increased Sequencing Coverage on Analyses of Human Genetic Variation"
nav_exclude: true
---
Group A17: Karthik Guruvayurappan, Michael Nodini, Maddie LaScola, Andrew Li

## Introduction 
The Introduction Will Go Here


## Background
Genome wide association studies (GWAS) allow for scientists to identify genetic variants associated with phenotypes like height or disease risk.
Expression quantitative trait loci (eQTLs) are genetic variants that are significantly associated with gene expression.1
eQTL associations are confounded by linkage disequilibrium (LD), where individual DNA positions are not inherited independently.
 Fine-mapping uses further statistical methods to pinpoint potential causal variants
Quantifying eQTL enrichment with functional annotations, such as ATAC-seq for accessible chromatin, provides a mechanism for determining eQTL function.4,5
Recent advances in the 1000 Genomes Project now provide higher sequencing coverage datasets.7


## Abstract

Genome-wide association studies determine associations between variants at individual genomic positions called single nucleotide polymorphisms (SNPs) and various phenotypes such as height or diabetes. Expression quantitative trait loci (eQTLs) are SNPs that are significantly associated with gene expression for a certain gene. The link between genetic variation and observable phenotypes is poorly understood, and eQTL analyses link genetic variation to gene expression that informs downstream phenotypes. These associations can be refined using downstream analyses like fine-mapping and functional annotation enrichment which can better locate causal variants across the genome. However, coverage, the amount of times each individual nucleotide is sequenced on average, is a major component in the power to detect SNPs. In this analysis, we combine the approach of eQTL analyses with both fine-mapping and functional annotation enrichment to compare a high-coverage and low-coverage dataset from a cohort in the 1000 Genomes Project.


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

### INSERT CONCLUSIONS HERE (IDEALLY BETTER COVERAGE = BETTER  RESULTS)

## References

1. Lappalainen, Nature (2013) 2. Pritchard, American Journal of Human Genetics (2001) 3. Hormozdiari, Genetics (2014) 4. Amariuta, American Journal of Human Genetics (2019) 5. Buenrostro, Current Protocols in Molecular Biology (2015) 6. Subramanian, Proceedings of the National Academy of Sciences (2005) 7. Byrska-Bishop, Cell (2022) 8. Purcell, American Journal of Human Genetics (2007) 9. Shabalin, Bioinformatics (2012) 10. Kundaje, Nature (2015)


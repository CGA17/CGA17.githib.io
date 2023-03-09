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
Genome wide association studies are a way for scientists to identify inherited genetic variants associated with risk of disease for a particular trait. This method studies the entire set of DNA, also known as a genome, from a population searching for small variations called single nucleotide polymorphisms also known as SNPs. These small variations can lead to an increased chance of developing diseases later in life such as lung cancer. Variations in genetic expression lead to altered production of proteins which alter the functions of cells inside the body. These small variations are responsible for changes as small as hair color up to life altering diseases. For example, sickle cell anemia stems from a mutation on a gene responsible for encoding the hemoglobin molecule on red blood cells. Due to the mutation, the red blood cells are formed in a sickle shape rather than round and can block blood flow leading to discomfort along with other afflictions. If these risks are discovered early on in one’s life preventative measures can be taken to decrease the likelihood of developing the disease or additional screenings can be scheduled to monitor an individual and catch the disease before it causes untreatable damage. Understanding how genetic expression translates to the observable traits we express is a necessary step towards providing insights for disease treatment, risk, prevention, and heritability.

Expression quantitative trait loci (eQTLs) are single nucleotide polymorphisms (SNPs) that are significantly associated with gene expression. Previous studies have applied linear models to associate genotype with gene expression and call eQTLs.1 The numerous resulting associations are significantly confounded by linkage disequilibrium (LD), and are therefore insufficient to determine causal relationships between SNPs and gene expression. Further methods development is required to determine functional significance from eQTL mapping. Fine-mapping provides a suite of methods to determine high-confidence SNPs likely to include causal variants, and can be performed with software tools such as CAVIAR. Quantifying eQTL enrichment with functional annotations, such as ATAC-seq for accessible chromatin,  provides another mechanism for determining eQTL power. For instance, eQTL enrichment with ATAC-seq can reveal cell-type specific eQTL strength. Genes with ATAC-seq enrichment for a given cell type can be analyzed with Gene Set Enrichment Analysis (GSEA) to reveal underlying cell type-specific biological pathways. Finally, recent advances in genome assembly published by the Telomere-to-Telomere (T2T) consortium have resulted in a complete human genome assembly, and have shown analysis improvements on the 1000 Genomes Project dataset. The genome assembly could have a significant impact on both the genotype and RNA-sequencing data obtained from the 1000 Genomes Project, which impacts downstream analysis like eQTL mapping. Reanalyzing eQTLs using this improved genome assembly could result in improved eQTL mapping and identification of causal SNPs. 



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

INSERT CONCLUSIONS HERE (IDEALLY BETTER COVERAGE = BETTER  RESULTS)

## References

1. Lappalainen, Nature (2013) 2. Pritchard, American Journal of Human Genetics (2001) 3. Hormozdiari, Genetics (2014) 4. Amariuta, American Journal of Human Genetics (2019) 5. Buenrostro, Current Protocols in Molecular Biology (2015) 6. Subramanian, Proceedings of the National Academy of Sciences (2005) 7. Byrska-Bishop, Cell (2022) 8. Purcell, American Journal of Human Genetics (2007) 9. Shabalin, Bioinformatics (2012) 10. Kundaje, Nature (2015)

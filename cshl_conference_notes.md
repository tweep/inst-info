
# Workshop notes 

## Workshop: Predicting Immunogenecity for proteins  

We're using RNAseq data from the SRA to call variants, then we call SNPs and see how the proteins are effected ( non-synonymous SNPs). We divide the region around the SNP's in 9-mers and use machine learning ( fred2 library ) to predict Immunogenecity for differnt classes, like MHC class I, MHC class II and tcell. 

We wrote a complete pipeline + prediction in 2.5 days and bundled it with docker.

## Wednesday evening: Useful scientifc software 
### Traditonal approaches, contemporary challenges 
Intro talks, 7:30 PM, 15 min per talk 

### Seeting : 
Isolated, on campus - minmal contact to the outside world.
See http://www.cshl.edu 
Cancer, Neuroscience, quantitative biology, plant biligy and bioinformatics and genomics.  

Cold Spring Harbor Laboratory (CSHL) is a private, non-profit institution with research programs focusing on cancer, neuroscience, plant genetics, genomics and quantitative biology.

It is one of 68 institutions supported by the Cancer Centers Program of the U.S. National Cancer Institute (NCI) and has been an NCI-designated Cancer Center since 1987.[3] The Laboratory is one of a handful of institutions that played a central role in the development of molecular genetics and molecular biology.[4]

It has been home to eight scientists who have been awarded the Nobel Prize in Physiology or Medicine. CSHL is ranked among the leading basic research institutions in the world in molecular biology and genetics.[5] The Laboratory is led by Bruce Stillman, a biochemist and cancer researcher. 

CHSL is partily NCI funded - so lots of people from NCBI. 
- head of dbSNP 
- Deanna Church / Senior director of applications @ 10x Genomics 

#### Session 1 - 7:30 PM 
Rafael A Irizarry  (Harvard, founder of Bioconductor ) opens the conference with nice talk. 

#### Paralell comptuing on Spark using ADAM 
Frank A Nnothaft ( Berkeley ) talks about ADAM and how they speed up the variant calling by doing a clean gatk rewrite in scalar / spark framework. They currently don't have a support for joint genotyping / joint variant discovery. He estimates his joint variant discovery tool will be published by the end of the year. 


#### Intro on bioinformatics tools 
- Biconductor talk from Martin. Talking about bioconductor and it's history. and the "hello ranges" - like Hello Kitty, just in R. 

#### Fabien - R notebooks  
R notebooks - benefits of having documentation + code together. 
- Introduction into R notebooks  
- comes with UI to annotate and modify visualizations   
MetaR takes advantage of Language Workbench Technology
- http://campagnelab.org/software/metaR/ 
- http://campagnelab.org/ ( read laboratory focus) 

#### Apollo Genome Annotation Tool  
Apollo is the first instantaneous, collaborative genomic annotation editor available on the web. 
Visualize genes in the Jbrowse viewer 
http://genomearchitect.org

### Machine learning 
#### Cellular response dsta
Barbara Engelhardt (Princetown University @ Chicago) explains how to analyze time-series expression data and how to interprete the response on A549 cell line. Classificaton of responses of geness in different clusters - meaning that different genes respond differently, with different time-repsonse curves - aim to understand gene regulation.
http://biorxiv.org/content/early/2016/09/09/074419   

The Engelhardt Group develops statistical models and methods for high-dimensional genomic data. In particular, we study human genetic variation and its impact on genomic regulation, including gene expression and splicing, with the goal of identifying mechanisms of human disorders and diseases. There are a wide range of projects in these areas in the group (see Research for more information), including:

Sparse factor analysis for estimating population structure, low-dimensional mapping of complex phenotypes, and gene co-expression analysis
Statistical models for improving power to detect trans-expression quantitative trait loci and small genetic effects
Alternative splicing and its role in complex phenotypes
Global approaches to estimate differential networks
Bayesian structured sparse regression for fine mapping of traits to genetic variants
Genome-wide association studies for pharmacogenomic, metabolic, and cardiovascular phenotypes

http://beehive.cs.princeton.edu/
 
#### 
Hhuang Y-F 
Overcoming "needle in the stack problem" when analyzing RNAseq data : Current individual predictors : conversataion, TBFS binding sites, functionaly assays.  

### Winner's curse  in qunatitative genmocds 
https://en.wikipedia.org/wiki/Winner%27s_curse 
http:/tinyurl.com/zjb92e 

### Avanti Shrikumar - DeepLift Neural Networks  
Neural networks go genomics - prediction of regulation of genes. 

The research focusses on development of statistical and machine learning methods for integrative analysis of diverse 
functional genomic and genetic data to learn models of gene regulation.  We have led the analysis efforts of the 
Encyclopedia of DNA Elements (ENCODE) and The Roadmap Epigenomics Projects with the development of novel methods for        

- Adaptive thresholding and normalization of massive collections of ChIP-seq and DNase-seq data
- Dissecting combinatorial transcription factor co-occupancy within and across cell-types
- Predicting cell-type specific enhancers from chromatin state profiles
- Exploiting expression and chromatin co-dynamics with to predict enhancer-target gene links

 Jointly modeling sequence grammars at regulatory elements and their chromatin state dynamics, expression 
 changes of regulators and functional interaction data to learn unified multi-scale gene regulation programs

- Elucidating the heterogeneity of chromatin architecture at regulatory elements 
- Improving the detection and interpretation of potentially causal disease-associated variants from 
  Genome-wide association studies


Algorithms for computing importance scores in deep neural networks. Implements the methods in "Learning Important Features Through Propagating Activation Differences" by Shrikumar, Greenside, Shcherbina & Kundaje.
Predicting sequence motifs - http://github.com/kundajelab/deeplift  
Ask for slides ...

#### Yulia Rubanova - Interpretation of mutational signatures 
http://cancer.sanger.ac.uk/cosmic/signatures

-> Use gene classifcation 


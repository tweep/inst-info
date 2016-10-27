
# Workshop notes 

## Workshop: Predicting Immunogenecity for proteins  

We're using RNAseq data from the SRA to call variants, then we call SNPs and see how the proteins are effected ( non-synonymous SNPs). We divide the region around the SNP's in 9-mers and use machine learning ( fred2 library ) to predict Immunogenecity for differnt classes, like MHC class I, MHC class II and tcell. 

We wrote a complete pipeline + prediction in 2.5 days and bundled it with docker.

## Wednesday evening: Useful scientifc software 
### Traditonal approaches, contemporary challenges 

Rafal Irizarry ( founder of Bioconductor ) opens the conference with nice talk. 

#### Paralell comptuing on Spark using ADAM 
Frank A Nnothaft ( Berkeley ) talks about ADAM and how they speed up the variant calling by doing a clean gatk rewrite in scalar / spark framework. They currently don't have a support for joint genotyping / joint variant discovery. He estimates his joint variant discovery tool will be published by the end of the year. 


#### Paralell comptuing on Spark using ADAM 


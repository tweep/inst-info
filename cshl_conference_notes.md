
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


    



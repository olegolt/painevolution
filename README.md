# The mismatch hypothesis for chronic pain – insights from ancient, comparative and neuroimaging genomics

![Last update](https://img.shields.io/badge/last_update-April_17,_2025-green)


***
Poster to be presented at EFIC 2025, Lyon <br>

contact: ole.goltermann@maxplanckschools.de

***


## Short summary

We aim to investigate the evolutionary history of common genetic variations that affect chronic overlapping pain conditions (COPC) and associated brain morphology in order to provide information to test the mismatch hypothesis for chronic pain.

## Methods

### 1. GWAS data
GWAS data for brain morphology is available here: https://open.win.ox.ac.uk/ukbiobank/big40/
GWAS data for chronic overlapping pain is available upon request here: https://academic.oup.com/brain/article/145/3/1111/6425672?login=true

### 2. Selected brain regions
GWAS summary statistics were downloaded for surface area of 46 brain regions, as these showed [statistically significant differences](https://pubmed.ncbi.nlm.nih.gov/37543299/)  between chronic overlapping pain patients and health controls. For these regions we calculated genetic correlations with GWAS data for COPC using LD score regression [ldsc](https://github.com/bulik/ldsc). p-values were bonferroni-corrected. In total, 17 out of 46 regions showed shared genetic variance between surface area and COPC diagnosis. These regions were used for later analysis of evolutionary influences on their genetic architecture. 

### 3. Evolutionary timescales for our analyses
In our study we aimed to investigate the evolutionary influence based on the following timescales/annotations.

1. Fetal human gained enhancers - [Reilly et al. 2015, *Science*](https://www.science.org/doi/10.1126/science.1260943)
2. Differentially Methylated Regions (DMRs) between anatomically modern humans and chimpanzees - [Gokhman et al. 2020, *Nat. Comm.*](https://www.nature.com/articles/s41467-020-15020-6)
3. DMRs between anatomically modern humans and archaic humans - [Gokhman et al. 2020, *Nat. Comm.*](https://www.nature.com/articles/s41467-020-15020-6)
4. Ancient selective sweep sites - [Peyregne et al. 2017, *Genome Res.*](https://pubmed.ncbi.nlm.nih.gov/28720580/)
5. Human Accelerated Regions - [Lindblad-Toh et al. 2011, *Nature*](https://www.nature.com/articles/nature10530)
6. Archaic deserts - [Vernot et al. 2016, *Science*)[https://pubmed.ncbi.nlm.nih.gov/26989198/]
7. Neandertal introgressed alleles - [Prüfer et al. 2017, *Science*](https://pubmed.ncbi.nlm.nih.gov/28982794/)
8. Selection pressure over the past 100 generations (Singleton density scores) - [Field et al. 2016, *Science*](https://www.science.org/doi/10.1126/science.aag0776)

### 4. Epigenetic influences
The following two annotations were used to detect epigenetic contributions to the genetic architecture of COPC and associated brain morphology measures.

1. Epigentic influences related to activity of the adaptive and innate immune system - [Stricker et al. 2024, *Cell Genom.*](https://pubmed.ncbi.nlm.nih.gov/38190103/)
2. fetal human active marks, calculated from the Roadmap Epigenomics Consortium - [Roadmap Epigenomics Consortium et al. 2015, *Nature*](https://www.nature.com/articles/nature14248)

### 5. Partitioned heritability analysis
We used LDSC partitioned heritability analysis to test heritability enrichment for the following annotations: 

1. fetal human gained enhancers
2. Archaic deserts
3. Neandertal introgressed alleles
4. Epigenetic influences related to activity of the adaptive and innate immune system
5. fetal human active marks

### 6. MAGMA gene set analysis 
Due to the small size of the remaining 4 evolutionary annotations, we used [MAGMA gene set analysis](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1004219) to test for gene enrichment.

### 7. Overlap analysis
We performed qualitative overlap analysis between statistically significant heritability enriched annotations and lead SNPs using GeneOverlap. 

### 8. Local genetic correlations
We performed local genetic correlations between GWAS data for COPC and the 17 selected brain regions using [LOGO Detect](https://github.com/ghm17/LOGODetect)




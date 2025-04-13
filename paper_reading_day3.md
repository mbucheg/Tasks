## What is CNV/CNA? 
Copy Number Variations/Copy Number aberrations: specific sequence repeats in the genome that vary between individuals. It is a form of structural variation and can be important in cancer development and progression. Sections of DNA can be duplicated or deleted. 
## How will you describe or introduce progenetix (scale, data source, cancer types and so on)?
Progenetix is a derived database that focuses on CNVs and provides mutation data related to cancer. The individual sample data is curated from different sources, with the majority coming from genomic arrays from SNP platforms, as well as from CGH experiments and whole genome/exome sequencing (WGS/WES) studies. As of now, the database includes **156,871 samples** across **906 distinct cancer types**. This open resource offers key features such as local CNV aberrations, as 
well as CNV cancer profiles and annotated references to research articles about cancer genome screening experiments.
## Describe NCIt, ICDO, UBERON codes, and their relationships.
*NcIt: National Cancer Institute thesaurus*
*ICDO:International Classification of Diseases in Oncology*
*UBERON: Uber-anatomy ontology*
## What are CNV segmentations and CNV frequencies and how to use them?
CNV segmentations are regions of the genome that are consistently altered.
CNV frequencies give the count of how often aspecific genomic region is altered across many samples.
CNV segmentations are great to analyse CNV data on the sample level, to see what genes are altered.
CNV frequencies are beneficial to identify cancer types or subtypes, and are used to find specific CNV abundances in cancer.
## What are APIs and how to use APIs in progenetix?
*Application Programming Interfaces:*
"set of routines, protocols and tools that specifies how software components interact, to exchange data and processing capabilities" This is a way you can access databases. ~ Source: BIO390:Lecture 1 
## How does progenetix visualize CNA profiles?
- CNV frequency plots using *pgxFreqplot* 
X-axis: Genomic positions (organized by chromosome).
Y-axis: Frequency (percentage of samples showing gain or loss at each position).
- Individual CNV profiles --> genome wide view for each biosample
- Genomic CNA Matrix View --> Heatmaps showing CNAs across multiple samples.
## What do you think should be improved in progenetix?



Source for all the answers to the questions:\
Qingyao Huang, Paula Carrio-Cordo, Bo Gao, Rahel Paloots, Michael Baudis, The Progenetix oncogenomic resource in 2021, Database, Volume 2021, 2021, baab043, <https://doi.org/10.1093/database/baab043> \
Progenetix Website <https://progenetix.org/>



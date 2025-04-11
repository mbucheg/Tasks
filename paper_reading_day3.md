## What is CNV/CNA? 
Copy Number Variations/Copy Number aberrations: specific sequence repeats in the genome that vary between individuals. It is a form of structural variation and can be important in cancer development and progression. Sections of DNA can be duplicated or deleted. 
## How will you describe or introduce progenetix (scale, data source, cancer types and so on)?
Progenetix is a derived database, that provides mutation data in cancer, especially highlighting the focus on CNVs. The individual sample data is curated from multiple different sources, the majority coming from genomic arrays from SNP platforms and from CGH experiments and WGS/WES studies.
Up to date: there are 156871 samples from 906 different cancer types.
The open resource offers key feautres like: Local CNV aberrations, as well as CNV cancer profiles and provides annotated references to research articles about cancer genome screening experiments
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
Application Programming Interfaces
"API: set of routines, protocols and tools that specifies how software components interact, to exchange data and processing capabilities" Source: BIO390:Lecture 1 
This is a way you can access databases.
## How does progenetix visualize CNA profiles?
- CNV frequency plots using *pgxFreqplot* 
X-axis: Genomic positions (organized by chromosome).
Y-axis: Frequency (percentage of samples showing gain or loss at each position).
- Individual CNV profiles --> genome wide view for each biosample
- Genomic CNA Matrix View --> Heatmaps showing CNAs across multiple samples.
## What do you think should be improved in progenetix?



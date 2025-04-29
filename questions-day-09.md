
# Questions BIO392 day 9
These questions are designed to test your understanding of the sequence analysis practical and the accompanying literature. Please change the name of this file to <First letter>-<Last name>-questions-day-09.md, and upload it to your folder in the course GitHub. Please submit before 13:00 on 6th May.
These questions will be graded. The most important thing is not that you get everything right, but that you show that you thought about the questions; so no copy/pasting!

### Q1
**What information do the CHROM, POS, REF, and ALT columns contain in a VCF file?**
* CHROM: Which chromosome are we on? It is identified via the reference genome.
  Chromosome 5
* POS: Which position contains a variant?
 1. Position 5:106700
 2. Position 5:137481
* REF: What is the nucleotide in the reference genome? A ‘.’ means there is no variant.
  1. a
  2. a
* ALT: What is the alternate allele of our sequence at this position?
  1. aa
  2. agagagaga

### Q2
**Using these four columns, how could you determine whether a sequencing sample contains a variant?**
* Check the ALT column and see which nucleotide is noted there.  
* To double-check you compare it with the base in the	REF column.

  If there's a nucleotide in the ALT column, then that would suggest there is a variant for that specific sequencing sample.\
  For patient 1, we find the 1st position from the last question that changes a>aa when there's a "1/1" in the patient 1 column. \
  For patient 3, it's the 2nd position from the last question that changes a>agagagaga. 

### Q3
**After loading all the files into IGV, there should be four different kind of tracks. Briefly explain what type of information each track contains**
* We have the tracks with the alignments of each patient. We see the different reads and their associated information when we click on them (read name, alignment start and map quality). At the top of each alignment we see a profile which could be the coverage of each base.
* We also have one track that represents the gene, with information on the source and the location on the chromosome that we are at. 
* Another one representing the transcript.
* And the last one “merged_results.vcf” contains the variant information for each patient.
  
- *Patient tracks*: Each patient shows the aligned reads from the corresponding BAM file. When it's grey, this means it aligns with the reference genome. The first line of the track that spans the whole chromosome with different levels is the coverage track, so how many reads cover each base.
- *Gene track*: shows us where the gene (in this case canonical APC from the WNT signaling pathway) is located within that chromosome.
- *Variant track*: has 4 different "rows" one for the reference, and the other three for the patients. This displays the different STRs in dark blue, and most importantly the variants we're interested in in turquoise. The variant then shows us the genotype and zygosity.
- *Transcript track*: transcript reference strand. Usually in IGV, there's a transcript track that shows the exons in dark blue boxes along the reference genome. However, in this case I couldn't find the transcript track, so only the reference sequence and the other three tracks.

### Q4
**Based on the VEP output, which of the STR variants you identified do you expect to have the most impact? Why?**
link = ![image](https://github.com/user-attachments/assets/f5f793bb-4997-4a7b-ad14-8bf68002ffc3)
I would expect the variant allele GAGAGAGA to have the most impact because it appears to be located within an exon, so it affects a protein-coding region. This variant seems to introduce a frameshift mutation, which often leads to nonsense mutations and the production of truncated proteins.
Nonsense-mediated decay (NMD) is a surveillance pathway that recognizes and degrades mRNAs with premature stop codons. Since many of the protein-coding transcripts of the APC gene are predicted to be targets of NMD, this could be detrimental to the Wnt signaling pathway, where APC plays a key regulatory role.
The other variant falls within an intron, making it less likely to affect protein function unless it disrupts splicing or regulatory elements.

Sources: \
[link = https://www.ensembl.org/Homo_sapiens/Tools/VEP/Results?tl=EJTwUWdceMoxAJtI-11001158] \
BCH 252: RNA and Proteins, Lecture 6: mRNA Degradation, Nonsense Mediated DEcay, Prof. Dr. Martin Jinek

### Q5
**What phenotype or disease do you expect this variant to be involved with?**
APC is a tumor suppressor gene, which is usually a negative regulator in Wnt signaling pathway. 
If this variant creates frameshifts, this could cause a problem of regulating the Wnt signaling pathway, as this is important for embryonic development, stem cell maintenance as well as organ and tissue (re-)generation. If the negative regulator protein is truncated and nonfunctional or gets degarded by NMD, then this makes the Wnt signaling pathway not controlled anymore, this could cause the stem cell maintenance to not be in control anymore, causing uncontrolled proliferation and thus abnormal cell growth, like cancer.


Sources \
Rim, E. Y., Clevers, H., & Nusse, R. (2022). The Wnt Pathway: From Signaling Mechanisms to Synthetic Modulators. Annual Review of Biochemistry, 91, 571-598. [link = https://doi.org/10.1146/annurev-biochem-040320-103615] \
[link = https://search.clinicalgenome.org/kb/genes/HGNC:583]


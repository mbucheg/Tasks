# Task: Estimate Storage Requirements for 1000 Genomes
 How much computer storage is required for 1000 Genomes?
 • WES & WGS: Whole Exome Sequencing/Whole Genome Sequencing
 • Different file formats
  • SAM: Sequence Alignment/Map
  • BAM: Binary Version of SAM
  • VCF: Variant Call Format
  • FASTA: Fast-All or originally Fast Alignment Search Tool – A

## Storage Estimates

### WGS vs WES (Per Genome)
| Type | BAM      | VCF      | FASTQ      | Total (approx.) |
|------|----------|----------|------------|-----------------|
| WGS  | 100  GB  |   1 GB   |  80  GB    |     ~180 GB     |
| WES  |   8  GB  | 0.1 GB   |  5   GB    |      ~12 GB     |

> Multiply by 1000 genomes:
- **WGS**: ~180 TB
- **WES**: ~12 TB

 • Associated costs
  • Cost factors
  • Raw Storage costs
 • Familiarize with VCF format
 ➡specification in article collection
Please provide 1 page size estimates and reasoning for the use of the different file types (i.e. which would you use for storing called variants, which for full archival purposes, browser visualisation), for 
3-5 formats. Submit your files (.md) per pull request to your Github directory.

Source: 
VCF <https://sequencing.com/blog/post/how-to-use-genome-sequencing-data-files?utm_source=chatgpt.com>
BAM size: <https://www.strand-ngs.com/support/ngs-data-storage-requirements>
COST BAM: <https://techcommunity.microsoft.com/blog/healthcareandlifesciencesblog/genomic-data-storage-in-azure-basic-compression-for-mapped-sequencing-data/3721670>
FASTA size: <https://biowize.wordpress.com/2012/04/27/can-i-estimate-genome-size-from-the-size-of-the-fasta-file/>

all: <https://3billion.io/blog/big-data-among-big-data-genome-data>

# Task: Estimate Storage Requirements for 1000 Genomes
 How much computer storage is required for 1000 Genomes? What are the associated costs?
 Please provide 1 page size estimates and reasoning for the use of the different file types (i.e. which would you use for storing called variants, which for full archival purposes, browser visualisation), for 3-5 formats.
 • WES & WGS: Whole Exome Sequencing/Whole Genome Sequencing
 • Different file formats
  • SAM: Sequence Alignment/Map
  • BAM: Binary Version of SAM
  • VCF: Variant Call Format
  • FASTA: Fast-All or originally Fast Alignment Search Tool – A

## Storage Estimates

### WGS vs WES (Per Genome)
| Type | BAM      | VCF      | FASTQ      | Total (approx.) | Multiply by 1000 genomes: |
|------|----------|----------|------------|-----------------|---------------------------|
| WGS  | 100  GB  |   1 GB   |  80  GB    |     ~180 GB     |           ~180 TB         |
| WES  |   8  GB  | 0.1 GB   |  5   GB    |      ~12 GB     |           ~12 TB          |

• Associated costs
  • Cost factors
  • Raw Storage costs

-  Google cloud (not recommended): 0.025 $ per GB per month in Zurich * 200'000 GB = 5000 $ for ~ 200 TB 
-  I found a NAS(Network attached storage) with 200TB for 7300 euros. See link: <https://anynas.de/nas-systeme/asustor/10-bay/asustor-as7110t/230084/asustor-as7110t-10-bay-200tb-bundle-mit-10x-20tb-ironwolf-pro-st20000nt001> \
 • Familiarize with VCF format

VCF: for storage of genome variants
BAM: archival purposes and browser visualization



Source: 
VCF <https://sequencing.com/blog/post/how-to-use-genome-sequencing-data-files?utm_source=chatgpt.com>
BAM size: <https://www.strand-ngs.com/support/ngs-data-storage-requirements>
COST BAM: <https://techcommunity.microsoft.com/blog/healthcareandlifesciencesblog/genomic-data-storage-in-azure-basic-compression-for-mapped-sequencing-data/3721670>
FASTA size: <https://biowize.wordpress.com/2012/04/27/can-i-estimate-genome-size-from-the-size-of-the-fasta-file/>
Google Cloud: <https://cloud.google.com/storage/pricing?utm_source=chatgpt.com&hl=de#europe>
all: <https://3billion.io/blog/big-data-among-big-data-genome-data>

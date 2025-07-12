# Analysis of OmpA-like Domains in Gram-Negative Bacterial Outer Membranes

## Project Overview
This repository contains bioinformatic and statistical workflows to investigate OmpA-like domain-containing proteins across five gram-negative bacteria:
- *Acinetobacter baumannii*  
- *Escherichia coli*  
- *Klebsiella pneumoniae*  
- *Pseudomonas aeruginosa*  
- *Vibrio cholerae*  

**Key Tools**: DIAMOND BLASTp, BLASTn, R  
**Objective**: Analyze conservation, functional roles, and evolutionary relationships of OmpA-like domains.

## Key Hypotheses Tested
1. Each species encodes multiple OmpA-like domain-containing proteins
2. A subset shows significant sequence similarity across species
3. Proteins with similar functions show higher sequence conservation
4. Some conserved proteins originate from distinct genetic backgrounds


## Bioinformatics Workflow

### 1. Data Preparation
- Downloaded reference genomes from NCBI RefSeq (see Table S1)
- Extracted OmpA-like domain sequences from ProSite (PS51123)
- Created FASTA files for each bacterial proteome

### 2. Workflow
- See genomic_lab_book.txt for full workflow

### 3. Figures
- See genomics-figures-script.R for creation of figures

## Data Provenance

### Genome Data Sources
All bacterial genome data was obtained from **NCBI RefSeq** with the following accession numbers:

| Species | Strain | Assembly Accession | Size | Data Type |
|---------|--------|--------------------|------|-----------|
| _Acinetobacter baumannii_ | ATCC 19606 | GCF_009035845.1 | 4 Mb | Complete genome |
| _Escherichia coli_ | K-12 substr. MG1655 | GCF_000005845.2 | 4.6 Mb | Complete genome |
| _Klebsiella pneumoniae_ | subsp. pneumoniae HS11286 | GCF_000240185.1 | 5.7 Mb | Complete genome |
| _Pseudomonas aeruginosa_ | PAO1 | GCF_000006765.1 | 6.3 Mb | Complete genome |
| _Vibrio cholerae_ | RFB16 | GCF_008369605.1 | 4.1 Mb | Complete genome |

**Download method**:  
All genomes were downloaded using NCBI Datasets with the following file types:
- Protein sequences (FASTA format)
- Annotation features (GFF format)

### Protein Domain Data
OmpA-like domain sequences were obtained from:
- **PROSITE database** (Expasy)  
  - Profile: PS51123 (OMPA_2)  
  - 82 sequences with 0 false positives  
  - Retrieved using ScanProsite tool  

**Exclusion**:  
OMPA_1 (PS01068) was excluded due to lower number of hits (56) and pattern-based search limitations.

## References

Sigrist, C.J.A., de Castro, E., Cerutti, L., Cuche, B.A., Hulo, N., Bridge, A., Bougueleret, L. and Xenarios, I. (2013) 'New and continuing developments at PROSITE', Nucleic Acids Research, 41(Database issue), pp. D344–D347. doi:10.1093/nar/gks1067.<img width="468" height="76" alt="image" src="https://github.com/user-attachments/assets/dd5419aa-cd12-4cb9-b933-a3f82a65f168" />





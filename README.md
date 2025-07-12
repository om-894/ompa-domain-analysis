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


# Phylogenetic Analysis of SARS-CoV-2 Lineages

Author: TALAPANTI VENKATA SRI TULASI
Course: BSc Bioinformatics (2nd Year)
Date: August 2026

## Project Overview
This project aims to visualize the evolutionary relationships between major SARS-CoV-2 variants (Early 2020, Delta, and Omicron). As a second-year undergraduate student, I built this pipeline to demonstrate fundamental skills in molecular phylogenetics and data curation.

## Dataset
Source: NCBI Virus Database.
Composition: 30 complete genomes curated from human hosts.
Selection: Sampled across three distinct timeframes:
  - 10 genomes from Early 2020 (Original/Alpha).
  - 10 genomes from mid-2021 (Delta).
  - 10 genomes from late 2021/early 2022 (Omicron).

## Methodology
1.  **Data Retrieval:** FASTA sequences were downloaded using the NCBI Virus Data Hub.
2.  **Multiple Sequence Alignment (MSA):** Sequences were aligned using the MUSCLE algorithm via MEGA software.
3.  **Phylogenetic Inference:** A Maximum Likelihood (ML) tree was constructed using the Tamura-Nei model with 100 bootstrap replicates to assess branch support.
4.  **Visualization:** The final tree was visualized and annotated in MEGA.

## Repository Contents
- `raw_data/`: The original FASTA file containing 30 sequences.
- `alignment/`: The saved MEGA alignment session (.mas).
- `results/`: The final phylogenetic tree in Newick format (.nwk) and PNG image.
- `README.md`: This project documentation.

## Key Results
- The phylogenetic tree robustly separates the 30 sequences into **three distinct monophyletic clades**.
- These clades correspond directly to the Early 2020, Delta, and Omicron variants.
- High bootstrap support values (92-100%) indicate strong statistical confidence in the branching patterns.

## Tools Used
- **MEGA (v12):** Alignment, ML tree construction, and visualization.
- **NCBI Virus:** Sequence retrieval and curation.

## How to Reproduce
1.  Clone this repository.
2.  Download and install MEGA software.
3.  Open `sars_cov_30_sequences.fasta` in MEGA.
4.  Follow the project workflow: Align → Build ML Tree → Visualize.

---
*Author's Note: This is a practical project completed to demonstrate proficiency in basic bioinformatics workflows for a Master's degree application.*


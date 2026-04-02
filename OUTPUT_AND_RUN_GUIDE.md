# Run and Output Guide

This document explains how to run the SARS-CoV-2 analysis workflow and where to find the final outputs.

## Project Goal
Analyze SARS-CoV-2 genomic sequences for three US states:
- California
- New York
- Texas

Main workflow notebook:
- bio-finall.ipynb

## Requirements
Install Python dependencies:

```bash
pip install -r requirements.txt
```

Recommended environment:
- Python 3.10+
- Jupyter Notebook or VS Code Notebook

## How To Run
1. Open bio-finall.ipynb
2. Run cells from top to bottom in order
3. Do not skip preprocessing cells because downstream steps depend on generated files
4. If a cell uses an absolute local path, replace it with your local project path

## Expected Core Outputs
After successful execution, these folders and files are the key outputs.

### State-specific outputs
- CALIFORNIA/
  - cleaned_California_data.csv
  - sequences.fasta
  - california_msa.fasta
  - consensus_california.fasta
  - tree_from_scratch.nwk
  - California_mutation_hotspot.png

- NEWYORK/
  - cleaned_New_York_data.csv
  - sequences.fasta
  - newyork_msa.fasta
  - consensus_newyork.fasta
  - tree_from_scratch.nwk
  - New York_mutation_hotspot.png

- TEXAS/
  - cleaned_Texas_data.csv
  - sequences.fasta
  - texas_msa.fasta
  - consensus_texas.fasta
  - tree_from_scratch.nwk
  - Texas_mutation_hotspot.png

### Combined/final outputs
- consenses/
  - consensus_california.fasta
  - consensus_newyork.fasta
  - consensus_texas.fasta
- final_consensus_tree.png
- phylogenetic_tree_cleaned.png

## Quick Validation Checklist
Use this checklist after running the notebook:
- All three cleaned CSV files exist in CALIFORNIA, NEWYORK, TEXAS
- All three consensus FASTA files exist in consenses
- At least one .nwk tree file exists per state folder
- final_consensus_tree.png and phylogenetic_tree_cleaned.png are generated

## Notes
- The repository excludes unrelated contour/pipe image artifacts by design.
- One very large file was intentionally excluded from version control to satisfy GitHub limits.

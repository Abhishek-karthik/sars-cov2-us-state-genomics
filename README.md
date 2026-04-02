# SARS-CoV-2 Genomic Analysis Across US States

This repository contains an end-to-end notebook workflow for analyzing SARS-CoV-2 genomic sequences from California, New York, and Texas.

## Project Scope
- Data extraction and filtering by state
- Sequence cleaning and FASTA export
- Alignment and guide-tree construction
- Consensus sequence generation
- Mutation hotspot visualization
- Comparative phylogenetic artifacts

## Main Notebook
- bio-finall.ipynb
- Detailed run and output guide: OUTPUT_AND_RUN_GUIDE.md

## Key Data and Output Folders
- CALIFORNIA
- NEWYORK
- TEXAS
- consenses

## Typical Outputs
- State-specific cleaned CSV and FASTA files
- Consensus FASTA sequences
- Multiple sequence alignment artifacts
- Newick tree files (.nwk)
- Plot images (.png/.jpg)

## Reproducibility
Install dependencies and run the notebook cells in order:

```bash
pip install -r requirements.txt
jupyter notebook
```

## License
No license has been set yet. Add a LICENSE file if you plan to share publicly.

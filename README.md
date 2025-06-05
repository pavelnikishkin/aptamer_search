# aptamer_search

🧬 Nanopore Aptamer Discovery Using Machine Learning
This project presents a reproducible pipeline for processing nanopore sequencing data to identify candidate aptamers using clustering and machine learning techniques.

Key features:

FASTQ parsing and primer-based aptamer extraction

Sequence clustering with isONclust and HDBSCAN

Embedding generation using the Nucleotide Transformer

Cluster quality evaluation (alignment score, entropy, outlier ratio)

Multiple sequence alignment and visualization (Clustal Omega + Jalview)

Final aptamer extraction with lab-tested results for SARS-CoV-2 spike protein

The entire pipeline is implemented in Python 3.10 using Jupyter Notebooks and open-source bioinformatics tools.

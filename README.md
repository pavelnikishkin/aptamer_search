# 🧬 Nanopore Aptamer Discovery Using Machine Learning

This repository contains the implementation of a pipeline for detecting aptamer candidates from raw nanopore sequencing data using clustering algorithms and transformer-based embeddings.

The study focuses on the identification of aptamers targeting the SARS-CoV-2 spike protein, based on data generated through **nanopore sequencing** and processed with modern **bioinformatics** and **machine learning** tools.

---

## 🔍 Overview

The pipeline performs the following steps:

1. **Parsing FASTQ files** with raw sequencing reads.
2. **Filtering reads** based on known primer sequences.
3. **Clustering sequences** using `isONclust` and optionally `HDBSCAN` on learned embeddings.
4. **Generating embeddings** using the pre-trained `Nucleotide Transformer` model.
5. **Evaluating clusters** with metrics such as alignment score, entropy, and outlier ratio.
6. **Extracting aptamer candidates** based on high-consistency clusters.
7. **Visualizing alignments** with Clustal Omega and Jalview.

All steps are implemented in a reproducible Jupyter Notebook and optimized for GPU acceleration where possible.

---

## 🗂️ Repository Structure

├── datasets/

│ ├── sample1.fastq

│ ├── sample2.fastq

│ ├── sample3.fastq

│ └── sample4.fastq

│

├── pipeline/

│ └── aptamer_search.ipynb

│

├── README.md

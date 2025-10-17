# CAFA 6 Protein Function Prediction

**Author:** Rethick CB  
**License:** CC BY-SA 4.0  

---

## Overview

This project implements a computational framework for predicting protein functions using amino acid sequences and hierarchical Gene Ontology (GO) annotations. The goal is to build models that can predict what a protein does based on its sequence, which is essential for understanding biological processes and disease mechanisms.

---

## Project Structure

data/                  # Folder containing all input datasets
├── train_sequences.fasta
├── train_terms.tsv
├── train_taxonomy.tsv
├── go-basic.obo
├── testsuperset.fasta
├── testsuperset-taxon-list.tsv
├── IA.tsv
└── sample_submission.tsv
notebooks/             # Jupyter notebooks for preprocessing and modeling
src/                   # Optional: Python scripts for functions and models
README.md
LICENSE
submission.tsv         # Example output file for Kaggle



---

## Getting Started

1. Clone the repository:
bash
git clone https://github.com/cbrethick/protein-function-prediction.git
cd protein-function-prediction

2.	Install dependencies:

pip install biopython obonet networkx matplotlib pandas numpy
	3.	Place all required datasets in the data/ folder.

  Usage
	1.	Run the main notebook notebooks/CAFA6_protein_function_prediction.ipynb.
	2.	Load and preprocess the data:
	•	Training sequences and annotations
	•	Test sequences
	•	Gene Ontology graph
	•	Information Accretion (IA)
	3.	Encode sequences for ML/DL models (optional: one-hot encoding).
	4.	Train ML/DL models (e.g., CNN, RNN, Transformers) to predict GO terms.
	5.	Generate predictions and save submission file (submission.tsv) in Kaggle-compatible format.

⸻

Submission Format

The final submission file should be a TSV file with two columns:

Protein                     GO
sp                          XXXX

Each row corresponds to a predicted GO term for a protein.

License

This project is licensed under CC BY-SA 4.0.




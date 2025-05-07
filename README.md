# Cultural Classification Project

## Project Description

The goal of the project is to classify entities into three cultural categories:

- **Culturally agnostic**
- **Culturally representative**
- **Culturally exclusive**

We compare two approaches:
- A **non-LM approach** based on SpaCy embeddings and numerical features from Wikidata/Wikipedia.
- A **language-model-based approach** using RoBERTa with custom classification heads.

## Contents

- `LM - No-LM code.ipynb`: Google colab notebook containing all code for data enrichment (of test set), training, and evaluation.
- `Report.pdf`: Final report describing the methodology, experiments, and results.
- `Features_extraction.ipynb`: Google colab notebook containing all code for data enrichment of train and validation set.

## Results Summary

| Model      | Accuracy | F1-score |
|------------|----------|----------|
| Non-LM     | 76.0%    | 76.0%    |
| RoBERTa    | 81.0%    | 79.8%    |

The RoBERTa model with a custom classification head outperforms all others.

## Data Sources

The datasets used in this project were made available on [Hugging Face](https://huggingface.co/datasets/sapienzanlp/nlp2025_hw1_cultural_dataset) by the TAs of the course of *Multilingual Natural Language Processing*.  
They include Wikidata entities annotated as culturally agnostic, culturally representative, or culturally exclusive.

## Authors

- A. Infantino - 1922069
- A. Di Chiara - 1938462
- F. Fragale - 2169937

---

This project was completed as part of Homework 1 for the course of Multilingual Natural Language Processing at Sapienza University of Rome.

## How to Use in Google Colab

To run this notebook on Google Colab, follow these steps:

1. Download this entire repository as a ZIP file from GitHub.
2. Upload the folder to your **Google Drive** (e.g., under `.../My Drive/Cultural-classification`).
3. At the beginning of the notebook, make sure to mount Google Drive and set the correct working directory:
4. Then run the notebook as usual.

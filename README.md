# Scientific Paper Text Summarization

## Overview
This project focuses on developing and evaluating text summarization models for scientific papers using transformer-based architectures. Given the increasing volume of academic publications, the need for efficient and high-quality summarization methods has become essential. This study compares different transformer models fine-tuned for summarizing biomedical articles, analyzing their effectiveness based on various evaluation metrics.

## Dataset
The dataset used in this project is derived from **PubMed Central® (PMC)**, a comprehensive repository of biomedical literature maintained by the U.S. National Library of Medicine. The dataset consists of:
- Full-text articles in structured **XML** format.
- Extracted abstracts and main content for summarization.
- Preprocessed and cleaned data stored in **JSON** format for model training.

## Models
The study evaluates and fine-tunes two transformer-based models specifically designed for handling long-text documents:

1. **BigBird-PEGASUS**
   - Optimized for processing long sequences using sparse attention mechanisms.
   - Combines the strengths of **BigBird** for long-text handling and **PEGASUS** for abstractive summarization.
   - Efficiently generates high-quality summaries by capturing key information.

2. **Longformer**
   - Uses a sliding window attention mechanism to efficiently process long documents.
   - Maintains computational efficiency while preserving contextual dependencies in lengthy texts.

## Evaluation Metrics
To assess the final quality of the generated summaries, we compare them against the original article abstracts using **Cosine Similarity** alongside the **ROUGE** metric. Cosine Similarity helps measure the semantic closeness between the generated summary and the reference abstract by analyzing their vector representations.

### Cosine Similarity
- Computes the **cosine of the angle** between the summary and original abstract vectors.
- Higher values indicate better semantic similarity and content retention.

### ROUGE Score
To ensure high-quality summarization, we employ the **ROUGE** (Recall-Oriented Understudy for Gisting Evaluation) metric:

- **ROUGE-1**: Measures **word-level** overlap.
- **ROUGE-2**: Evaluates **phrase-level** coherence.
- **ROUGE-L**: Captures **sentence structure** consistency.

Higher ROUGE scores indicate **better summary accuracy, coherence, and fluency**.

## Contributors

- **[Hana Esfandiar](https://github.com/Hana-esf)** - Co-Researcher  
- **[Modjtaba Rouhani](https://scholar.google.com/citations?user=nPuuMikAAAAJ&hl=en)** - Supervisor Professor
---

This repository contains the Jupyter Notebook used for data preprocessing, model fine-tuning, and evaluation. Contributions and suggestions for further improvements are welcome!

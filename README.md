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

### Cosine Similarity
- Computes the **cosine of the angle** between the summary and original abstract vectors.
- Higher values indicate better semantic similarity and content retention.

## Evaluation Metrics
To assess the quality and effectiveness of the generated summaries, the project employs the **ROUGE** (Recall-Oriented Understudy for Gisting Evaluation) metric:

- **ROUGE-1**: Measures the overlap of unigrams (single words) between the reference and generated summary.
- **ROUGE-2**: Evaluates the overlap of bigrams (two-word sequences) for capturing phrase-level similarities.
- **ROUGE-L**: Considers the longest common subsequence (LCS) to measure sentence-level structural similarity.

Higher ROUGE scores indicate better summarization performance, with an emphasis on maintaining key information while ensuring fluency and coherence.

## Contributors

- **[Hana Esfandiar](https://github.com/Hana-esf)** - Co-Researcher  
- **[Modjtaba Rouhani](https://scholar.google.com/citations?user=nPuuMikAAAAJ&hl=en)** - Supervisor Professor
---

This repository contains the Jupyter Notebook used for data preprocessing, model fine-tuning, and evaluation. Contributions and suggestions for further improvements are welcome!

# Topic Modeling Comparison: LDA vs. BERTopic on arXiv CS Abstracts

This repository contains the code and documentation for a comparative study of two topic modeling techniques—**Latent Dirichlet Allocation (LDA)** and **BERTopic**—applied to a dataset of arXiv Computer Science (CS) abstracts. The project evaluates the performance of these models based on coherence, topic diversity, outlier handling, and qualitative interpretability, with the goal of identifying their suitability for analyzing diverse scientific abstracts.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Discussion Points](#discussion-points)
- [Contributing](#contributing)
- [License](#license)

## Project Overview
This project compares two topic modeling approaches:
- **LDA**: A traditional probabilistic model that identifies topics based on word co-occurrence patterns.
- **BERTopic**: A modern approach leveraging transformer-based embeddings for semantic topic discovery.

The comparison is conducted on a dataset of 136,238 arXiv CS abstracts, evaluating:
- **Quantitative Metrics**: C_v coherence and topic diversity (1 - average Jaccard similarity).
- **Qualitative Aspects**: Interpretability of topics and visualization insights.
- **Outlier Handling**: How each model manages documents that do not fit well into topics.
- **Computational Efficiency**: Preprocessing intensity and tuning complexity.

The code is implemented in Python using libraries like `gensim`, `bertopic`, `nltk`, `pandas`, and visualization tools (`pyLDAvis`, `matplotlib`, `seaborn`).

## Dataset
The dataset (`arXiv_scientific dataset.csv`) contains 136,238 arXiv CS abstracts with the following columns:
- `id`, `title`, `category`, `category_code`, `published_date`, `updated_date`, `authors`, `first_author`, `summary`, `summary_word_count`.

**Note**: The dataset is not included in this repository due to size constraints. Users must provide their own copy of the dataset in the project directory.

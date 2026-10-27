# Tech Job Recommender (NLP)

[![Python](https://img.shields.io/badge/Python-3-3776AB?logo=python&logoColor=white)](https://www.python.org)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-TF--IDF-F7931E?logo=scikitlearn&logoColor=white)](https://scikit-learn.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-F37626?logo=jupyter&logoColor=white)](https://jupyter.org)
[![License](https://img.shields.io/badge/License-MIT-green)](LICENSE)

A content-based recommender that suggests tech job openings for a candidate profile using TF-IDF and cosine similarity.

## Table of Contents

- [About](#about)
- [Dataset](#dataset)
- [Pipeline](#pipeline)
- [Getting Started](#getting-started)
- [Documents](#documents)
- [Team](#team)
- [License](#license)

## About

Project for the Artificial Intelligence course of the Information Systems program at
Universidade Presbiteriana Mackenzie (2026), taught by Prof. Dr. Leandro Zerbinatti.
The system receives a candidate's resume as text and ranks job postings by similarity
to it. The work continued in
[tech-job-recommender](https://github.com/EnzoFerroni/tech-job-recommender), which adds
filtering, bigrams and model tuning. Documents and notebooks are in Portuguese.

## Dataset

[AI-Powered Job Recommendations](https://www.kaggle.com/datasets/samayashar/ai-powered-job-recommendations/data)
(Kaggle): 50,000 job postings across industries, locations, experience levels and
salary ranges. Main fields used: job title, required skills, industry and experience
level.

## Pipeline

The full pipeline is in
[`notebooks/Sistema_Recomendacao_Completo.ipynb`](notebooks/Sistema_Recomendacao_Completo.ipynb):

1. Load the dataset and run exploratory analysis
2. Clean and normalize text (lowercase, punctuation removal)
3. Vectorize the skills text with TF-IDF
4. Rank postings by cosine similarity to the candidate profile
5. Evaluate with Precision@5

## Getting Started

```bash
git clone https://github.com/EnzoFerroni/job-recommender-nlp.git
cd job-recommender-nlp
pip install pandas scikit-learn matplotlib seaborn jupyter
jupyter notebook notebooks/
```

## Documents

- Report: [`docs/ProjetoIA.pdf`](docs/ProjetoIA.pdf)
- Presentation video: [YouTube](https://www.youtube.com/watch?v=U4bau8jKEr0)

## Team

- Enzo Ferroni ([@EnzoFerroni](https://github.com/EnzoFerroni))
- Leonardo Rodrigues
- Rafael Neves

## License

Code and documents are released under the [MIT License](LICENSE). The dataset belongs
to its Kaggle author and is redistributed under its original terms.

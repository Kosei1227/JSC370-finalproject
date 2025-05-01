# Embedding-Based Trend Analysis of NeurIPS Publications (1987–2024)

This project analyzes publication trends and topic evolution within papers accepted at the NeurIPS conference from 1987 through 2024. Leveraging state-of-the-art embedding and clustering methods (SPECTER2 embeddings, UMAP dimensionality reduction, and HDBSCAN clustering), we identify historical and recent trends, topic growth patterns, and research directions within the machine learning community.

---

## Project Overview

The analysis comprises three main components:

- **Data Acquisition and Cleaning:**  
  Scraping paper titles and abstracts from NeurIPS proceedings website, followed by data preprocessing and filtering.

- **Embedding and Clustering:**  
  Semantic embeddings via SPECTER2 model, dimensionality reduction with UMAP, and clustering with HDBSCAN.

- **Trend Modeling:**  
  Time-series regression models (linear regression, ridge regression, random forest, and gradient boosting) to evaluate and predict the growth and decline of topics.

Interactive visualizations allow detailed exploration of topic dynamics and publication characteristics over the analyzed period.

---

## Reproducing the Analysis (Recommended: Google Colab)

Due to computational intensity (particularly embedding and clustering steps), we strongly recommend using **Google Colab** with GPU acceleration to reproduce results efficiently.

### Installation and Build Instructions

Run the following commands to build the Jupyter Book locally:

```bash
pip install sphinx-design    # critical dependency
jupyter-book clean . --all
jupyter-book build .
```

Alternatively, open and execute notebooks directly on Google Colab for straightforward replication.


Live website: **<https://kosei1227.github.io/JSC370-finalproject/>**

This site hosts my Jupyter-Book report, interactive Plotly dashboards, and all source code.


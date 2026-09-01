# Machine Learning for scRNA-seq Cell Type Classification

## Overview

Cell type annotation is an essential step in single-cell RNA sequencing (scRNA-seq) analysis. In this project, machine learning methods are used to predict immune cell types directly from single-cell gene expression data.

The classification task includes three cell populations:
- Activated CD4+ T cells
- NK cells
- Naive CD20+ B cells

The project combines exploratory data analysis, dimensionality reduction, unsupervised clustering, supervised machine learning, model optimization, and model interpretation.

## Workflow
The analysis includes:

1. Data exploration and preprocessing
2. Feature scaling
3. Feature selection
4. Dimensionality reduction using PCA
5. Non-linear visualization using t-SNE and UMAP
6. K-means clustering and cluster evaluation
7. Supervised cell-type classification
8. Hyperparameter optimization using cross-validation
9. Model evaluation on held-out test data
10. Feature importance and model interpretation

## Machine Learning Models

The following classifiers were explored:
- Random Forest
- Logistic Regression
- K-Nearest Neighbors (KNN)

Hyperparameter optimization was performed using 5-fold cross-validation with macro F1-score as the optimization metric.

## Results

The optimized model achieved strong performance on the held-out test set:

- **Accuracy:** 0.99
- **Macro F1-score:** 0.99
- **CD4+ T activated F1-score:** 0.98
- **NK F1-score:** 0.98
- **Naive CD20+ B F1-score:** 1.00

The final model used a Random Forest classifier with feature selection and hyperparameter optimization through 5-fold cross-validation.


## Dimensionality Reduction & Clustering

The project explores:
- Principal Component Analysis (PCA)
- t-SNE
- UMAP
- K-means clustering
- Silhouette score
- Elbow method

These methods were used to investigate whether transcriptionally similar cells naturally form groups corresponding to their biological cell types.

## Model Interpretation

To understand which genes contribute most strongly to cell-type predictions, the project includes:
- Logistic regression coefficients
- Random Forest feature importance
- ELI5
- LIME local explanations

## Technologies

- Python
- pandas
- NumPy
- scikit-learn
- matplotlib
- seaborn
- UMAP
- LIME
- ELI5


## Repository Structure

```text
scRNA-cell-type-classification/
├── scRNA_cell_type_classification.ipynb
└── README.md
```
<img width="830" height="587" alt="Project visualization" src="https://github.com/user-attachments/assets/fcd93127-6f20-4f41-93a9-b96d402089d3" />


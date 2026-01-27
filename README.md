# Principal Component Analysis (PCA)

## Overview

This repository contains a Jupyter Notebook that demonstrates **Principal Component Analysis (PCA)**, a widely used **dimensionality reduction technique** in machine learning and data analysis. The notebook focuses on understanding why PCA is used, how it reduces dimensions, and how it helps visualize high-dimensional data.

---

## Table of Contents

1. Installation  
2. Project Structure  
3. Why PCA is Used  
4. PCA Implementation  
5. Explained Variance  
6. Visualization  

---

## Installation

Install the required Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn
```

---

## Project Structure

- `PCA.ipynb` – Notebook demonstrating PCA implementation and visualization

---

## Why PCA is Used

PCA is used to:
- Reduce the number of features while retaining important information
- Remove multicollinearity between features
- Improve visualization of high-dimensional data
- Reduce computational cost

PCA transforms original features into **principal components**, which are uncorrelated variables.

---

## PCA Implementation

The notebook applies PCA using `scikit-learn`.

Basic commands used:
```python
from sklearn.decomposition import PCA

pca = PCA(n_components=2)
X_pca = pca.fit_transform(X)
```

---

## Explained Variance

Explained variance indicates how much information each principal component captures.

Key points:
- Helps decide the number of components
- Higher variance means more information retained

Common command:
```python
pca.explained_variance_ratio_
```

---

## Visualization

The notebook includes visualization of data after dimensionality reduction.

Example:
```python
plt.scatter(X_pca[:, 0], X_pca[:, 1])
```

This helps understand how PCA separates data in lower dimensions.

---


## Author

**Manasa Vijayendra Gokak**  
Graduate Student – Data Science  


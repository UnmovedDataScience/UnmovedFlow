## Overview

**UnmovedFlowV2** is an extensive Python class, focusing on streamlining data preprocessing, feature engineering, model fitting, evaluation, and ensemble methods for both regression and classification problems. It supports data splitting, generation of sample datasets, imputation, encoding, scaling, dimensionality reduction (with PCA, t-SNE, and UMAP), and outlier removal. For model development, it integrates with popular machine learning algorithms from Scikit-learn and XGBoost, and offers cross-validation and grid search capabilities for hyperparameter tuning. Additionally, it features data visualization tools for insights into data relationships and model performance.

**UnmovedV1** is the original, purely functional code I am working on replacing with UnmovedflowV2.

**UnmovedV2** is class based.

## Quick Start

To get started with UnmovedFlowV2 on Kaggle, Colab, or locally, execute the following commands:

```python
import os
import nbformat

# URL to download
url = "https://github.com/UnmovedDataScience/UnmovedFlow/raw/main/UnmovedFlowV2.ipynb"
filename = "UnmovedFlowV2.ipynb"

# Attempt to use wget, if it fails, download using requests
wget_success = os.system(f'wget {url} -O {filename}')

if wget_success != 0:
    # If wget fails (returns non-zero exit status), use the Python-based method
    import requests

    response = requests.get(url)
    with open(filename, 'wb') as f:
        f.write(response.content)

# Execute the notebook
with open(filename) as f:
    notebook = nbformat.read(f, as_version=4)

for cell in notebook.cells:
    if cell.cell_type == 'code':
        exec(cell.source)
```

## Alternative Local Installation

If you prefer not to download UnmovedFlow each time from GitHub, you can:

1. Download the `UnmovedFlowV2.ipynb` notebook
2. Open it and a separate notebook in the same Jupyter IDE.

Then, run the following command in your separate notebook:

```python
%run "./UnmovedFlowV2.ipynb"
```
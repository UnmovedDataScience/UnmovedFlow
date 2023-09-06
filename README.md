# UnmovedFlow: A Framework for Tabular Regression & Classification

## Overview

UnmovedFlow aims to make working with tabular data for regression and classification tasks simpler and more efficient. The framework is highly customizable, allowing you to easily modify functions to fit your specific needs.

## Examples

For practical implementations of UnmovedFlow, visit our Kaggle profile:

- [UnmovedFlow Kaggle Examples](https://www.kaggle.com/unmoved/code)

## Quick Start

To get started with UnmovedFlow on Kaggle, Colab, or locally, execute the following commands:

```python
!wget https://github.com/UnmovedDataScience/UnmovedFlow/raw/main/UnmovedFlow.ipynb

import nbformat

with open('UnmovedFlow.ipynb') as f:
    notebook = nbformat.read(f, as_version=4)

for cell in notebook.cells:
    if cell.cell_type == 'code':
        exec(cell.source)
```

## Alternative Local Installation

If you prefer not to download UnmovedFlow each time from GitHub, you can:

1. Download the `UnmovedFlow.ipynb` notebook
2. Open it and a separate notebook in the same Jupyter IDE.

Then, run the following command in your separate notebook:

```python
%run "./UnmovedFlow.ipynb"
```

You can also download `TEST_DUMMY.ipynb` to test this locally. Make sure both notebooks are in the same directory or specify the path as needed.

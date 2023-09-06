# UnmovedFlow
A Framework For Tabular Regression &amp; Classification

For several examples of UnmovedFlow in usage in the wild, visit our Kaggle profile:
https://www.kaggle.com/unmoved

UnmovedFlow is designed to be very easy to edit if needed.
If you need to change the way any of the functions work simply copy the corresponding function (and libraries) from the UnmovedFlow notebook into your Kaggle, Colab, or Local notebook and redefine it as needed before running it.


To use Unmovedflow Directly in Kaggle or Colab or Locally run

!wget https://github.com/UnmovedDataScience/UnmovedFlow/raw/main/UnmovedFlow.ipynb

import nbformat

with open('UnmovedFlow.ipynb') as f:
    notebook = nbformat.read(f, as_version=4)
    
for cell in notebook.cells:
    if cell.cell_type == 'code':
        exec(cell.source)

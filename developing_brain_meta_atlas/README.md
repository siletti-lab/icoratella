### Developing brain meta-atlas

The files uploaded in this folder explain how I worked on the training dataset after the filtering carried with Cytograph. 

**1: `from_noAdolescence_to_final_training_dataset.ipynb`**

This notebook is the main file. It provides a summary of the steps taken to transform the dataset generated through the iterative application of the Cytograph pipeline into the final dataset used for training the Random Forest and Mahalanobis distance-based classifiers. While this notebook outlines each step of the process, the actual analyses were conducted in separate notebooks, and the resulting data was incorporated here. For reproducibility, I will reference the specific notebooks used to generate the imported data at each step.

**2: `DEA_of_cytograph_clusters.ipynb`**

In this notebook, I analyzed the clusters stored in the anndata object from `...noAdolescence.h5ad` to assign labels to them. This process involved retrieving the top 25 marker genes for each cluster and overlaying known markers on the UMAP visualization of the training dataset.

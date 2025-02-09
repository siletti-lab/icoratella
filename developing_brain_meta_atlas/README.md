### Developing brain meta-atlas

The files uploaded in this folder explain how I worked on the training dataset after the filtering carried with Cytograph. 

**1: `from_noAdolescence_to_final_training_dataset.ipynb`**

This notebook is the main file. It provides a summary of the steps taken to transform the dataset generated through the iterative application of the Cytograph pipeline into the final dataset used for training the Random Forest and Mahalanobis distance-based classifiers. While this notebook outlines each step of the process, the actual analyses were conducted in separate notebooks, and the resulting data was incorporated here. For reproducibility, I will reference the specific notebooks used to generate the imported data at each step.

**2: `DEA_of_cytograph_clusters.ipynb`**

In this notebook, I analyzed the clusters stored in the anndata object from `...noAdolescence.h5ad` to assign labels to them. This process involved retrieving the top 25 marker genes for each cluster and overlaying known markers on the UMAP visualization of the training dataset.

**3: `gIPC_reannotation_eliminating_astro.ipynb`**

In this notebook, I performed a clustering analysis on Cluster 9, previously annotated as gIPCs, obtained from the Cytograph pipeline. The analysis was necessary because the UMAP visualization suggested that Cluster 9 contained cells that likely belonged to astrocytes. Upon further investigation, this assumption was confirmed.

**4:  `gIPC_reannotation_after_removing_astro.ipynb`**

To do this, I loaded the anndata file `noAdolescence_nocc_noclusters_SecondManualAnnotations.h5ad`, which contains the updated annotations generated in the `gIPC_reannotation_eliminating_astro.ipynb` notebook. Then, I performed a clustering analysis on the newly defined gIPCs, to see if it was possible to refine the annotation into pre-OPCs and pre-Astrocytes.

**5:  `extracting_interneurons.ipynb`**

In this notebook, I loaded the Braun Anndata object `human_dev_GRCh38-3.0.0.h5ad` and selected some subcortical interneurons, to integrate them into the main notebook with the developing brain meta-atlas. This integration aims to enhance the diversity and accuracy of cell type annotations in the developing brain meta-atlas.

**6:  `fixing_metatadata_of_training_dataset.ipynb`**

This notebook loads, visualizes, and annotates multiple versions of the training dataset, focusing on standardizing key metadata columns for consistency.

**7:  `DEA_of_cell_classes.ipynb`**

In this notebook, I analyzed the manual annotation stored in the column 'ThirdManualAnnotation' from noAdolescence_nocc_noclusters_ThirdManualAnnotations_Interneurons.h5ad, retrieving the top 25 marker genes for each label.


**8:  `clustering_analysis_scanpy_noAdolescence.ipynb`**

I reanalyzed the dataset using the scanpy pipeline to validate the results obtained with Cytograph, after eliminating some clusters and cc genes (noAdolescence_nocc_noclusters_FirstManualAnnotations), generated in notebook 1. Specifically, I preprocessed, integrated, and clustered the dataset, and generated all the panels for Figure S1.

**9:  `Figure_7_A_B_C_D_and_S2.ipynb`**

In this notebook I generated the different panels of Figure 7 and Figure S2.

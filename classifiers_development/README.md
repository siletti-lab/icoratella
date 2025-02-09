### Classifiers development

The files uploaded in this folder explain how I developed the Random Forest classifier and the Mahalanobis distance-based classifiers.

**1: `Random_Forest_training_and_Figure_13.ipynb`**

In this script, I trained the Random Forest classifier and saved the model to disk. This allows the model to be utilized for testing in `Random_Forest_testing.ipynb`. Here I also generated **Figure 13** of the report.

**2: `Random_Forest_testing.ipynb`**

In this notebook, I applied the Random Forest classifier—previously trained in `Random_Forest_training_and_Figure_13.ipynb` and saved to disk—to the GBM dataset. Additionally, I evaluated the results by identifying the most important genes for each class.

**3: `Mahalanobis_training_and_figure_15.ipynb`**

In this script, I trained the Mahalanobis distance-based classifier and saved the model to disk. Then, I computed the "important genes" for the classification. This allows the model to be utilized for testing in `Mahalanobis_testing.ipynb`. I also generated **Figure 15** of the report.


**4: `Mahalanobis_testing.ipynb`**

In this code, I used the Random Forest classifier—previously trained in `Mahalanobis_training_and_figure_15.ipynb` and saved to disk—to analyze the GBM dataset. 


**5: `Random_Forest_Figure_9.ipynb`**

In this notebook, I generated the panels for Figure 9 of the report.


**6: `Random_Forest_Figure_11_12_and_unpublished.ipynb`**

In this notebook, I generated the panels for Figures 11 and 12 of the report, and some images that I did not include. These images show the results on sample SL040 of Random Forest classification of GBM dataset.


**7: `Random_Forest_Figure_17C_and_unpublished.ipynb`**

In this notebook, I generated the panel C for Figure 17 of the report, and some images that I did not include. These images show the results on sample KS414 of Random Forest classification of GBM dataset.


**8: `Mahalanobis_Figure_10.ipynb`**

In this notebook, I generated the panels for Figure 10 of the report. These images show the general results of Mahalanobis distance-based classification of GBM dataset.


**9: `Mahalanobis_Figure_14_and_unpublished.ipynb`**

In this notebook, I generated the panels for Figures 14 of the report, and some images that I did not include. These images show the results on sample SL040 of Mahalanobis classification of GBM dataset.


**10: `Mahalanobis_Figure_17D_and_unpublished.ipynb`**

In this notebook, I generated the panel C for Figure 17 of the report, and some images that I did not include. These images show the results on sample KS414 of Mahalanobis classification of GBM dataset.


**11: `Mahalanobis_accuracy.ipynb`**

In this script, I trained a Mahalanobis distance-based classifier using 80% of the training dataset and evaluated its performance on the remaining 20% by computing accuracy and other relevant metrics.


**12: `combined_MD_RF_statistics_and_Figures.ipynb`**

In this script, I generated figures and statistics to compare the outputs of these two classification methods, as produced in Random_Forest_testing.ipynb and Mahalanobis_testing.ipynb.


**13: `predictions_using_sc_scores.ipynb`**
I computed gene scores for the key genes using Scanpy's sc.tl.score_genes function and generated additional predictions. These predictions were then compared to the other predictions and integrated with the clustering analysis.

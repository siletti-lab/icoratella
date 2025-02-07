### Classifiers development

The files uploaded in this folder explain how I developed the Random Forest classifier and the Mahalanobis distance-based classifiers.

**1: `Random_Forest_training.ipynb`**

In this script, I trained the Random Forest classifier and saved the model to disk. This allows the model to be utilized for testing in `Random_Forest_testing.ipynb`.

**2: `Random_Forest_testing.ipynb`**

In this notebook, I applied the Random Forest classifier—previously trained in `Random_Forest_training.ipynb` and saved to disk—to the GBM dataset. Additionally, I evaluated the results by identifying the most important genes for each class.

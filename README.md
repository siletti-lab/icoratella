# Classifying Glioblastoma cells based on developmental cell type resemblance
#### Code used for the study

In this repository, you will find the code used in my study, organized into three main sections: *meta-atlas manipulation*, *classifiers development* and *GBM_manipulation (tumor clustering analysis)*.

Here's a brief summary of my work.

![graphical abstract ](https://github.com/siletti-lab/icoratella/blob/main/graphical_abstract.png)

Tumors are heterogeneous entities exhibiting a variety of cell types in complex spatial configurations, complicating the analysis of tumor composition and origin. The genetic and phenotypic diversity of cancer cells hides the initial mutations and cellular behaviors that lead to tumorigenesis, making it challenging to trace their evolutionary paths. Single-cell RNA sequencing has shed light on this heterogeneity, demonstrating that tumor cells often mirror specific developmental lineages. Therefore, identifying resemblances between tumor cells and specific healthy developmental cell types provides a starting point for a better understanding of tumor cell characteristics, helping to navigate tumor heterogeneity and potentially enhancing our understanding of tumorigenic processes. 

Despite these advances, most single-cell analyses that compare healthy and Glioblastoma cells rely on relatively small datasets or a single classification metric, often correlation-based, thereby limiting the robustness of their conclusions. This underscores the need for larger, more comprehensive datasets and the use of multiple analytical approaches that can validate each other’s findings. 

In this study, we systematically classified Glioblastoma cells by assessing their resemblance to various developmental cell types. For this purpose, we created a single-cell RNA sequencing meta-atlas encompassing multiple brain regions and developmental stages, then compared these data against an unprecedentedly large, unpublished single-cell Glioblastoma dataset. Two complementary methodologies were employed: a machine learning approach based on a Random Forest classifier, and a distance-based approach using the Mahalanobis distance. By evaluating consistency across these two techniques, we refined the classification process. Our findings suggest that while some tumor cells mimic specific developmental cell types, mainly Astrocytes, pre-Astrocytes and Oligodendrocyte Precursor Cells, others exhibit more complex transcriptional signatures requiring deeper investigation.

The new information on tumor composition will be used to explore how a tumor's cellular makeup is related to its clinical features—such as growth rate, treatment response, and prognosis—as well as its molecular characteristics, like clonal structure. Furthermore, making this classification reliable and systematic may enhance our understanding of how these cells co-opt developmental pathways to foster tumor growth.

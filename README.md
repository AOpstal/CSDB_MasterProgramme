## CSDB_MasterProgramme
This repository contains the R-scripts used to analyse and create the figures for my report.

## 20241002_MFI_FACS_analysis:
This script was created to perform Median Fluorescence Intensity analysis of 9 macrophage markers on monocyte-derived macrophages.
It contains the code to create the boxplots of my report.
M2-like macrophage markers: CD163, CD206.
M1-like macrophage markers: CD80, CD86, HLADR.
General macrophage markers: CD11b, CD14, CD16, CD64.

## 20241002_Macrophages_FACS_Analysis
This script was created to perform high parameter flow cytometry analysis to visualise the effect of all 9 markers combined.
It contains the code to create the PCAs and UMAPs of my report.
This script has been adapted from a tutorial from Vera Poort (van Boxtel group PMC) and Rico Hagelaar (van Boxtel group PMC). 
High parameter flow cytometry analysis using dimensional reduction algorithms.
The original R-script for this processing and analysis was kindly provided by the Van Boxtel group (Princess Máxima Center for pediatric oncology) and is available here: https://github.com/ProjectsVanBox/TallFlow.
.fcs files were processed as described in Poort, et al. 2024 (1).
With the following adjustments:
Ncell was adjusted to the amount of the condition with the lowest cells available.
PCA was additionally coloured for Experiments/Donors and for treatment conditions to ensure no skewing happened based on Experiment/Donors if the same conditions were present in these experiments.
Dimensional reduction using UMAP was the final step for our analysis as it was used for visualisation.
For UMAP, n was increased, n_iter was decreased due to computational limitations, and n_threads was decreased to 1. 
UMAP was additionally coloured for all conditions and all experiments/donors, for M0-, M1-, and M2-like macrophages, and each condition with M0-, M1-, and M2-like macrophages.   
all created plots with colour were saved.



## Reference
1. Poort, V. M., Hagelaar, R., Roosmalen, M. J. van, Trabut, L., Buijs-Gladdines, J. G. C. A.
M., Wijk, B. van, Meijerink, J. & Boxtel, R. van. (2024). Transient Differentiation-State
Plasticity Occurs during Acute Lymphoblastic Leukemia Initiation. Cancer Research,
84(16), 2720–2733. https://doi.org/10.1158/0008-5472.can-24-1090.



---
title: Item#14
layout: home
parent: 5. Feature Processing
nav_order: 3
---

### Item #14
“Removal of non-robust features” [1]  (licensed under CC BY)

### Explanation
“Whether unstable features are removed via test-retest, reproducibility analysis by analysis of different segmentations, or stability analysis [i.e., image perturbations]. Instability may be due to random noise introduced by manual or even automated image segmentation or exposed in a scan-rescan setting. The specific methods used should be clearly presented, with specific results for each component in multi-step feature removal pipelines.” [1]  (licensed under CC BY)

“This item is conditional. It is applicable only for the studies having tabular data (i.e., numeric radiomic features in a tabulated format, which is usually seen in hand-crafted and some deep learning-based studies as deep features).” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “To account for center-level differences, we used the Kruskal-Wallis test to identify features significantly associated with the center of origin. Subsequently, to assess radiomic feature reproducibility due to inter-reader variability, we sampled 36 cases from the training set, and all three radiologists (N.B., F.C., and F.L.) performed segmentations. Features significantly affected by segmentation-level differences, as determined by Mann-Whitney U tests, were excluded from the analysis. Benjamini-Hochberg corrections were applied to adjust the significance levels for multiple testing and reduce the false discovery rate. The features deemed robust for center and segmentation were then taken to the second step comprising supervised feature selection using the MSI status outcome.” [2] (licensed under CC BY)

> **Example #2:** “The re-annotated whole tumour ROIs and automatically generated maximum tumour area ROI were subjected to ICC test to assess stability concerning whole tumour (3D and 3DBB) and maximum tumour area (2D and 2DBB) features. Features with the ICC > 0.75 were included for subsequent analysis.” [3] (licensed under CC BY)

> **Example #3:** “To ensure the stability of the radiomic features extracted from the CT images, the segmentation and feature-extraction process was repeated in 80 randomly selected patients with CRMs from the training set. Intraclass correlation coefficients (ICCs) were used to evaluate consistency across the radiomic features; features with ICCs >0.75 were considered stable and were included in this analysis.” [4] (licensed under CC BY-NC)

### Hypothetical negative examples
> **Example #4:** Radiomic features were extracted from the segmented tumor regions using a standard feature-extraction pipeline. Collinear features were removed and all the remaining features were then used for model training.

> **Example #5:** We performed feature selection using LASSO regression. Features with coefficients of zero were removed.

> **Example #6:** Radiomic features were extracted from the images and ranked based on their importance in a random forest model. To avoid overfitting, we kept only the top 50 features.

### Importance of the item
The removal of non-robust features is crucial in radiomics to enhance the reliability and reproducibility of predictive models. Non-robust features, often influenced by variability in image acquisition, segmentation, or noise, can introduce instability and reduce model generalizability. Techniques such as test-retest analysis, reproducibility testing across different segmentations, and stability evaluation through image perturbations are used to identify and eliminate these unstable features related to different potential sources of noise (e.g., scanner, acquisition protocol, or segmentation process) [5]. By focusing on robust features, studies ensure that their models are less prone to overfitting and more likely to perform consistently in diverse settings [1]. This step is particularly relevant for tabular data, where handcrafted or deep features are extracted, as such data are highly susceptible to variability stemming from different imaging or preprocessing conditions [5].

### Specifics about the positive examples
The provided examples demonstrate how authors removed non-robust features in their analysis. Example #1 emphasizes a robust methodology to account for variability at different levels (center-level and inter-reader). The Kruskal-Wallis test identifies features influenced by the center of origin, while the Mann-Whitney U test screens features for inter-reader segmentation variability, and features significantly affected by these differences were excluded from the analysis. In Example #2 and Example #3, the feature stability is assessed through intraclass correlation coefficients (ICCs), and features with ICCs >0.75 are considered reliable and included for further analysis to enhance consistency.

### Specifics about the negative examples
Example #4 removes collinear features but does not test feature stability across different segmentations or test-retest settings. Example #5 applies LASSO regression for feature selection but only removes features with zero coefficients, without explicitly testing for reproducibility or robustness. Example #6 selects features based on their importance in a random forest model, prioritizing predictive power over stability, without assessing segmentation variability or test-retest consistency. These approaches focus on feature selection rather than ensuring feature robustness, making them inadequate under item #14.

### Recommendations for appropriate scoring
Studies should be scored based on their explicit description and application of methods to identify and remove non-robust features. Full points should be awarded if the study uses rigorous approaches like test-retest, perturbation analysis, or reproducibility testing across different segmentations and provides detailed results for each step in the feature removal pipeline. Studies that do not consider feature robustness or fail to report methods for removing unstable features should not receive points.
This item should not be confused with item #15. While item #15 focuses on selecting features that provide non-redundant information to reduce dimensionality, the current item (i.e., item #14) emphasizes the reliability and robustness of feature values.

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Bodalal Z, Hong EK, Trebeschi S, et al (2024) Non-invasive CT radiomic biomarkers predict microsatellite stability status in colorectal cancer: a multicenter validation study. European Radiology Experimental 8:98. https://doi.org/10.1186/s41747-024-00484-8
3. 	Zhu Y, Wei Y, Chen Z, et al (2024) Different radiomics annotation methods comparison in rectal cancer characterisation and prognosis prediction: a two-centre study. Insights Imaging 15:211. https://doi.org/10.1186/s13244-024-01795-5
4. 	Huang L, Ye Y, Chen J, et al (2023) Cystic renal mass screening: machine-learning-based radiomics on unenhanced computed tomography. dir 0:0–0. https://doi.org/10.4274/dir.2023.232386
5. 	Van Timmeren JE, Leijenaar RTH, Van Elmpt W, et al (2016) Test–Retest Data for Radiomics Feature Stability Analysis: Generalizable or Study-Specific? Tomography 2:361–365. https://doi.org/10.18383/j.tom.2016.00208
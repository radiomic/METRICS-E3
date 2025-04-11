---
title: Item#17
layout: home
parent: 5. Feature Processing
nav_order: 6
---

### Item #17 
“Robustness assessment of end-to-end deep learning pipelines.” [1]  (licensed under CC BY)

### Explanation
“Whether DL pipeline consistency of performance has been assessed in a test-retest setting, for example by a scan-rescan approach, use of segmentations by different readers, or stability analysis [i.e., image perturbations]. The specific methods used should be clearly presented.” [1]  (licensed under CC BY)

“This item is conditional. It is applicable only for the studies employing a DL pipeline for the entire feature extraction, processing and modeling process (e.g., computer vision models such as convolutional networks or transformers), without explicit conversion of DL-based image features to a tabular format for further processing or analysis.” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “We investigated the DL model performance using FGSM, PGD, and BIM adversarial image generation methods across different levels of pixel perturbation. To evaluate the performance of the DL models on adversarial images, we generated adversarial test sets by applying adversarial attacks on the original clean test sets. We measured relative susceptivity to adversarial images by determining the smallest perturbation ε required for adversarial images to generate a different output.” [2] (licensed under CC BY-NC-ND)

> **Example #2:** “To evaluate the impact of manual lesion cropping on model performance, a second radiologist (J.G.) with 1 years of experience reading MSK plain film independently recropped the images in the external test set, and model performance was evaluated on the external test set using this set of recropped images.” [3] (licensed under CC BY-NC-ND)
>
>“Comparison of model performance on the images in the external test set cropped by the original radiologist (Y.H.) and the second radiologist (J. G.) demonstrated no significant difference (Cohen's kappa score of 0.560 versus 0.549, p = 0.67).” [3] (licensed under CC BY-NC-ND)

> **Example #3:** “The test-retest reproducibility of the model output was studied in 34 axial or coronal T2 sequences from 17 ADPKD subjects who were scanned twice within a 3-week interval, short enough so that no changes in liver cyst number or volume were expected.” [4] (licensed under CC BY-NC)

> **Example #4:** “To evaluate the stability of the deep learning networks, we tested robustness against test–retest scenarios as well as inter-reader variations in input seed annotations. We used the publicly available test–retest RIDER dataset comprising 32 patients with lung cancer, each of whom underwent 2 chest CT scans within 15 minutes using the same imaging protocol and in a similar position. Using this dataset, we evaluated the stability of network predictions between the test and retest scans. A high stability was demonstrated (ICC = 0.91) between both predictions.

To assess stability against inter-reader variations in input data, we randomly relocated the input seed points in 3D space around the center of the tumor. This randomly shifts the network inputs during testing and can be regarded as simulating multiple human readers annotating the tumor’s center, with the inevitable variability among them. The network outputs show high correlation (Spearman’s rank-order correlation = 0.88). We also observed a high stability in prognostic predictions (AUC, μ = 0.68, σ = 0.014).” [5] (licensed under CC BY)

### Hypothetical negative examples
> **Example #5:** To assess robustness, we retrained the model five times with different random seeds and reported the average accuracy.

> **Example #6:** We used extensive data augmentation during training, including random rotations, flips, and brightness adjustments, to improve model robustness.

> **Example #7:** We achieved high accuracy on an external test set from a different institution, demonstrating the model's robustness.

### Importance of the item
Robustness can be defined as the relative stability of a target with respect to specific interventions on a modifier [6]. Although the term has many interpretations in machine learning, it usually refers to a model's adaptability to variations in input data, such as noise, adversarial perturbations, or shifts in distribution. If region of interest segmentation (e.g., cropping, semantic labeling) are included in the input data, these can also be the object of robustness analysis (e.g., manual labeling by different readers, automated perturbations). Without robustness checks, models can be unreliable in high-stakes applications, where they face varying inputs and updates over time. Assessing robustness helps identify and mitigate vulnerabilities, enabling more reliable, fair, and generalizable models [7].

### Specifics about the positive examples
In Example #1, robustness against adversarial attacks was measured using FGSM, PGD, and BIM methods.  Example #2 demonstrates robustness through the impact of manual lesion cropping on model performance. Example #3 evaluates test-retest reproducibility over a three-week interval, and, in Example #4, robustness is assessed using test-retest scenarios as well as inter-reader variations to test model stability. 

### Specifics about the negative examples
Example #5, which involves retraining the model multiple times with different random seeds, addresses variability due to model initialization rather than robustness against data variations or real-world perturbations. Example #6 emphasizes extensive data augmentation during the training phase, which might enhance model generalization but does not constitute a post-training robustness assessment against systematic perturbations or reproducibility conditions. 

Similarly, Example #7 focuses solely on model accuracy on an external test set, reflecting external validation and generalizability but not explicitly evaluating consistency under controlled perturbations or test-retest scenarios essential for robustness assessment.

### Recommendations for appropriate scoring
To get the item score, the study should clearly describe the robustness assessment strategies in the manuscript. A well-documented strategy should explain the types of robustness tests performed (e.g., adversarial attacks, test-retest reproducibility), the dataset modifications used to simulate real-world conditions, and quantitative metrics for robustness evaluation, such as stability scores or perturbation thresholds.

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Joel MZ, Umrao S, Chang E, et al (2022) Using Adversarial Images to Assess the Robustness of Deep Learning Models Trained on Diagnostic Images in Oncology. JCO Clinical Cancer Informatics e2100170. https://doi.org/10.1200/CCI.21.00170
3. 	He Y, Pan I, Bao B, et al (2020) Deep learning-based classification of primary bone tumors on radiographs: A preliminary study. eBioMedicine 62:103121. https://doi.org/10.1016/j.ebiom.2020.103121
4. 	Chookhachizadeh Moghadam M, Aspal M, He X, et al (2024) Deep learning-based liver cyst segmentation in MRI for autosomal dominant polycystic kidney disease. Radiology Advances 1:umae014. https://doi.org/10.1093/radadv/umae014
5. 	Hosny A, Parmar C, Coroller TP, et al (2018) Deep learning for lung cancer prognostication: A retrospective multi-cohort radiomics study. PLoS Med 15:e1002711. https://doi.org/10.1371/journal.pmed.1002711
6. 	Freiesleben T, Grote T (2023) Beyond generalization: a theory of robustness in machine learning. Synthese 202:109. https://doi.org/10.1007/s11229-023-04334-9
7. 	Liu J, Jin Y (2023) A comprehensive survey of robust deep learning in computer vision. Journal of Automation and Intelligence 2:175–195. https://doi.org/10.1016/j.jai.2023.10.002

[Back](https://radiomic.github.io/METRICS-E3/docs/Feature%20Processing%20(Con%204-5%20Item%2014-17)/Item%2016.html){: .btn .btn-purple  .mr-5  }
[Next](https://radiomic.github.io/METRICS-E3/docs/Preparation%20for%20Modeling%20(Item%2018-19)/Item%2018.html){: .btn .btn-purple   }


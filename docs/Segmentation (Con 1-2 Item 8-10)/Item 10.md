---
title: Item#10
layout: home
parent: 3. Segmentation
nav_order: 6
---

### Item #10 
“Test set segmentation masks produced by a single reader or automated tool” [1]  (licensed under CC BY)

### Explanation
“Whether final segmentation in the test set is produced by a single reader (manually or with a semi-automated tool) or an entirely automated tool, to better reflect clinical practice.” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “Subsequently, the same radiologist performed manual lesion segmentation using a dedicated software (ITKSNAP, v3.8.0) obtaining 2D regions of interest (ROIs) (Fig. 1). To assess feature stability, manual segmentation was also performed independently by two senior radiology residents (A.V. and A.V.) on 30 randomly selected patients from the training set in order to calculate feature intraclass correlation coefficient (ICC).” [2] (licensed under CC BY)

> **Example #2:** “Using 3D U-net-based DL algorithms as detailed in Supplementary Material 2 and Fig. S1, automated segmentation of liver and HCC lesions was conducted on each transverse section of T2-weighted imaging (T2WI), IP, opposed phase (OP), arterial phase (AP), portal venous phase (PVP), and delayed phase (DP; for MRI with extracellular contrast agent [ECA]) or translational phase (TP; for MRI with hepatobiliary contrast agent [HCA]) images […] Lesion segmentation was achieved using a 3D-UNet framework, characterized by an encoder-decoder architecture with 3D convolutions and pooling layers.” [3] (licensed under CC BY)

### Hypothetical negative examples
> **Example #3:** Tumor regions of interest (ROIs) were delineated on the pre-treatment CT images. The primary oncologist responsible for each patient's care performed the initial segmentation. These segmentations were then reviewed and adjusted as needed by a senior radiologist with 15 years of experience in gastrointestinal imaging.

> **Example #4:** Prostate lesions were segmented on T2-weighted MRI images using a commercially available deep-learning-based software. The software automatically generated segmentation masks. Any segmentations that were deemed inaccurate upon visual inspection by two radiology specialists in consensus were manually corrected.

### Importance of the item 
Manual segmentation is often considered the reference standard for the extraction of radiomic features in numerous studies. However, manual segmentation is time-consuming and in real-world practice, in light of the intense workload on radiologists’ shoulders, it is unlikely that multiple radiologists perform this task for a single patient and automated segmentation would be preferred to avoid an increase of current workload. For this reason, for studies requiring region of interest segmentation in the test set, having this task performed by a single reader or an automated tool is a better representation of real-world practice in the adoption of radiomics models, and provides a more accurate estimate of model performance Training data can be handled differently, and consensus segmentation by multiple readers can provide a stronger reference standard in some scenarios. Therefore, please note this item is exclusively focused on test data.

### Specifics about the positive examples
Example #1 states that the region of interest (ROI) was contoured by a single radiologist. Additionally, a second reader segmented a small subset of target lesions for a reproducibility analysis. However, these lesions were only included in the training set, meaning the test set patients appear to have been segmented solely by the original reader. Example #2 represents a fully automatic segmentation process with no human intervention, making it a strong example of automation in segmentation.

### Specifics about the negative examples
Example #3 describes a review process in which a second reader influences the final segmentation. The senior radiologist’s adjustments mean that the final segmentation is not solely the product of a single reader. This collaborative approach introduces a consensus-like element, violating the item’s requirement for either a single-reader or a fully automated segmentation process.

In Example #4, while the study initially employs an automated tool, the key issue is the manual correction step, where two additional readers modify the results. If only a single reader had corrected the automated segmentation, it would have been considered a semi-automated approach and would have met the item requirement. However, the involvement of multiple readers introduces an additional layer of human intervention, making it inconsistent with the criteria.

### Recommendations for appropriate scoring
Item #10 can be scored “Yes” if a single reader manually or semi-automatically performed the segmentation throughout the entire study or if a fully automated algorithm was used. However, for studies involving multiple segmentations for reproducibility analyses, it must be explicitly stated that these cases belong only to the training set, ensuring a clear separation from the test set.

Consensus segmentation or reviewing segmentations for accuracy does not meet the criteria for this item and should be scored “No”. Additionally, caution is advised when assessing automatic segmentation. Any intervention in the resulting segmentation by an automated tool renders it semi-automated; if such modifications involve more than one reader, the study should be scored “No”.

Importantly, if a study does not include a test set and relies solely on a resampling method, it should be clarified that all cases in the validation or test folds were segmented by a single reader (manually or semiautomatically) or an automated tool. This means that the entire dataset should be segmented either by a single reader or fully automated.

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Romeo V, Cuocolo R, Apolito R, et al (2021) Clinical value of radiomics and machine learning in breast ultrasound: a multicenter study for differential diagnosis of benign and malignant lesions. Eur Radiol 31:9511–9519. https://doi.org/10.1007/s00330-021-08009-2
3. 	Wei H, Zheng T, Zhang X, et al (2024) MRI radiomics based on deep learning automated segmentation to predict early recurrence of hepatocellular carcinoma. Insights Imaging 15:120. https://doi.org/10.1186/s13244-024-01679-8

[Previous: Item #9](https://radiomic.github.io/METRICS-E3/docs/Segmentation%20(Con%201-2%20Item%208-10)/Item%209.html){: .btn .btn-purple  .mr-5  }
[Next: Condition #3](https://radiomic.github.io/METRICS-E3/docs/Image%20Processing%20and%20Feature%20Extraction%20(Con%203%20Item%2011-13)/Condition%203.html){: .btn .btn-purple   }


---
title: Item#26
layout: home
parent: 8. Testing
nav_order: 1
---

### Item #26
“Internal testing” [1]  (licensed under CC BY)

### Explanation
“Whether the model is tested on an independent data set that is sampled from the same source as the training and/or validation sets.” [1]  (licensed under CC BY)

### Positive examples from the literature 
> **Example #1:** “Two hundred and ninety-three patients from the First Hospital of Wenzhou Medical University (Centre1) were randomised 7:3 into the training cohort (n = 205) and internal validation cohort (n = 88).” [2] (licensed under CC BY)

> **Example #2.** “From November 2013 to September 2021, we included 128 consecutive eligible patients with CD from our institution […] The final enroled patients were randomly allocated into training and test cohorts in an approximate ratio of 3:1 for developing and validating the RMs, respectively.” [3] (licensed under CC BY).

> **Example #3.** “This study retrospectively collected 794 cases of hypertensive cerebral hemorrhage diagnosed and treated by the Chongqing Emergency Medical Center and the Affiliated Hospital of Zunyi Medical University from January 2017 to July 2023. To achieve a balance between images and data, all cases are randomly divided into a training set and a validation set at 7:3. A retrospective collection of 77 cases of HICH treated at the People’s Hospital of Guizhou Province from June 2018 to March 2023 was conducted as the test set.” [4] (licensed under CC BY).

### Hypothetical negative examples
> **Example #4:** We trained our radiomic signature on a dataset of 450 patients diagnosed with liver cancer between 2015 and 2020 at X Hospital. Model performance was assessed using 10-fold cross-validation exclusively within this dataset. The average AUC across the folds was reported as the final performance metric.

> **Example #5:** A radiomics model predicting treatment response was developed using imaging data from 300 patients treated at University Hospital Center A (UHC-A). To validate the model, we collected prospective data from 85 patients treated with the same protocol at Regional Medical Center B (RMC-B) and used this as our test set.

### Importance of the item
Machine learning models are commonly used to analyze radiomics data. These models perform differently in the same population as the one used for training (usually perform better in this population), compared to an unseen population with different characteristics as the one used for training. Models encountered in literature have been usually tested by means of one of three methods: cross-validation [5], holdout internal testing and/or external testing. Cross-validation and internal testing involve the use of data from the same population (same hospital or random sample from multiple hospitals) as the training set, whereas external testing involves data from a population with different characteristics. Literature terms vary in the use of the terms “validation” and “testing” so both “internal testing” and “internal validation” have been interchangeably used. According to the CLEAR guideline for radiomics research and CLAIM 2024 update, internal testing should be established as terminology to avoid confusion [6, 7]. It should be noted that model testing is not the typical use case of cross-validation (which is a resampling technique designed to optimize the tuning/validation of a pipeline or model, as implied by its name). Therefore, extra attention needs to be placed on how cross-validation is implemented to ensure it matches the requirements of testing (no bias due to information leakage, e.g., fully nested data analysis pipeline) rather than validation (allows some degree of bias, intended either to compare different hyperparameter configurations or different models).

### Specifics about the positive examples
Example #1 presents a study with a randomly selected holdout “internal validation cohort”. This equates to an internal test set. The authors in Example #2 recruited consecutive patients which they randomly split 3:1 to “validate” the model. Since the “validation” set came from the same population as the training set it is considered as “internal testing”. Example #3 refers to a study utilizing a training, a “validation” and a “test” set. In this case the “validation” set is used for internal testing and the “test” set for external testing.

### Specifics about the negative examples
Example #4 relies solely on cross-validation within the training data. It lacks a separate, independent holdout dataset drawn from the same source to serve as a dedicated internal test set. 

In Example #5, the test set comes from a different institution (RMC-B) than the training set (UHC-A). This constitutes external testing, not internal testing, as the test data is not sampled from the same source population as the training data.

### Recommendations for appropriate scoring
When evaluating radiomics papers, care needs to be taken to understand which parts of the population have been used for training, internal or external testing. In any case the test set comes from the same place or cohort as the training set, the study should be scored positive in the “internal testing” item.

Cross-validation is a method for model tuning and performance estimation within the training process and does not constitute an internal or external test. On the other hand, nested cross-validation can satisfy internal testing if it includes distinct phases for training, validation, and final testing. In such cases, the final test set in the outer loop can be considered an internal test set.

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Zhu Y, Wei Y, Chen Z, et al (2024) Different radiomics annotation methods comparison in rectal cancer characterisation and prognosis prediction: a two-centre study. Insights Imaging 15:211. https://doi.org/10.1186/s13244-024-01795-5
3. 	Zhang M, Zeng Y, Fang Z, et al (2024) MRI radiomics enhances radiologists’ ability for characterizing intestinal fibrosis in patients with Crohn’s disease. Insights Imaging 15:165. https://doi.org/10.1186/s13244-024-01740-6
4. 	Yu F, Yang M, He C, et al (2024) CT radiomics combined with clinical and radiological factors predict hematoma expansion in hypertensive intracerebral hemorrhage. Eur Radiol 35:6–19. https://doi.org/10.1007/s00330-024-10921-2
5. 	Bradshaw TJ, Huemann Z, Hu J, Rahmim A (2023) A Guide to Cross-Validation for Artificial Intelligence in Medical Imaging. Radiology: Artificial Intelligence 5:e220232. https://doi.org/10.1148/ryai.220232
6. 	Kocak B, Baessler B, Bakas S, et al (2023) CheckList for EvaluAtion of Radiomics research (CLEAR): a step-by-step reporting guideline for authors and reviewers endorsed by ESR and EuSoMII. Insights into imaging 14:75. https://doi.org/10.1186/s13244-023-01415-8
7. 	Tejani AS, Klontzas ME, Gatti AA, et al (2024) Checklist for artificial intelligence in medical imaging (CLAIM): 2024 update. Radiology Artificial intelligence 6:e240300. https://doi.org/10.1148/ryai.240300

[Previous: Item #25](https://radiomic.github.io/METRICS-E3/docs/Metrics%20and%20Comparison%20(Item%2020-25)/Item%2025.html){: .btn .btn-purple  .mr-5  }
[Next: Item #27](https://radiomic.github.io/METRICS-E3/docs/Testing%20(Item%2026-27)/Item%2027.html){: .btn .btn-purple   }

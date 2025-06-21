---
title: Item#25
layout: home
parent: 7. Metrics and Comparison
nav_order: 6
---

### Item #25 
“Comparison with simple or classical statistical models” [1]  (licensed under CC BY)

### Explanation
“Whether a comparison with a simple baseline reference model (such as a Zero Rules/No Information Rate classifier) was performed. Use of machine learning methods should be justified by proof of increased performance. In any case, the comparison should be done with an appropriate statistical method (e.g., DeLong’s test for AUC comparison, Net Reclassification Index). Furthermore, in case of multiple comparisons, multiple testing correction methods (e.g., Bonferroni, Benjamini–Hochberg, or Tukey) should be considered in order to reduce the false discovery rate provided that the statistical comparison is done with a frequentist approach (rather than Bayesian).” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “Given the tabular nature of the data, expected number of instances available, and previous experiences, also following the recommendations made by the scikit-learn developers, a Random Forest (RF) ensemble algorithm was selected for this classification task. […]
> 
> Its accuracy was also compared to a baseline reference value (no information rate, NIR) corresponding to the accuracy obtainable by classifying all lesions as belonging to the most frequent class (i.e., the mode of the classes). […]
> 
> RF’s accuracy results are significantly better than the NIR (p = 0.0098).” [2] (licensed under CC BY)

> **Example #2:** “We built 8 different clinical-radiomics models based on k-nearest neighbor (KNN), RF, support vector machine (SVM), logistic regression (LR), Decision Tree (DT), Gradient Boosting Decision Tree (GBDT), AdaBoost, and extreme gradient boosting (XGBoost) [18, 20]. Finally, we compared the performance of these models. […]
> 
> All statistical tests were two-sided, and Bonferroni-corrected P-values were used to identify the characteristic significance of multiple comparisons.” [3] (licensed under CC BY)

> **Example #3:** “For building the radiomics-based models, we selected four well-established and methodologically diverse ML classifiers, namely the RF, LASSO, and SVM with radial basis function, and boosted generalized linear models (Boosted GLM). […]
> 
> Models’ performance in terms of ROC AUC was compared using DeLong’s test, and p-values less than 0.05 were considered significant. Due to multiple comparisons, Bonferroni correction was used to adjust the significance threshold and control the overall Type I error rate.” [4] (licensed under CC BY)

### Hypothetical negative examples
> **Example #4:** ...To evaluate the optimal approach for classifying glioma grade, we implemented and compared three distinct deep learning architectures: a standard 3D Convolutional Neural Network (3D-CNN), a Residual Network (ResNet) adaptation, and a Vision Transformer (ViT) model tailored for volumetric medical data. All models were trained on our institutional dataset (n=450) and evaluated on an external validation cohort (n=110). Performance was assessed using the Area Under the Receiver Operating Characteristic Curve (AUC). The ViT model achieved the highest AUC of 0.92, followed by the ResNet (AUC = 0.90) and the standard 3D-CNN (AUC = 0.88). While the ViT demonstrated the best performance numerically, further studies are needed to confirm its clinical utility...

> **Example #5:** ...We developed a Random Forest (RF) model utilizing 85 radiomic features extracted from pre-treatment CT scans to predict patient response to immunotherapy. For benchmarking, we also trained a Logistic Regression (LR) model using the same feature set. The models were evaluated on an independent test set (n=95). The RF model achieved an accuracy of 76% and an AUC of 0.81. The LR model showed an accuracy of 72% and an AUC of 0.77. The No Information Rate (predicting the majority class 'non-responder') yielded an accuracy of 65%. Our results suggest the RF model provides better predictive performance than the simpler LR model and baseline chance...

### Importance of the item
Comparing radiomic or deep learning models to simple or classical statistical models is essential to demonstrate their true added value. Without such comparisons, it becomes unclear whether complex techniques offer any meaningful advantage over basic approaches. Simple models, such as logistic regression or Zero Rules classifiers, often perform surprisingly well, particularly in small datasets. By applying proper statistical tests, such as DeLong’s test or Net Reclassification Index, researchers can objectively assess performance gains, ensuring that increased model complexity is scientifically justified rather than arbitrarily applied.

### Specifics about the positive examples
Example #1 provides a comparison with the no-information rate, which is supported by formal statistical testing. Examples #2 and #3 compare the performance of several algorithms, from simple to complex. These comparisons include statistical tests with multiplicity correction to evaluate the relative performance of the algorithms. While these two examples do not feature a no-information rate or zero-rule classifier, they incorporate simpler statistical models. Specifically, Example #2 includes a logistic regression model, and Example #3 uses a regularized linear regression model known as LASSO.

### Specifics about the negative examples
Example #4 fails because it only compares complex deep learning models (CNN, ResNet, ViT) with each other. It lacks a comparison to any simple or classical baseline model (like logistic regression or a No Information Rate) and also omits any formal statistical tests (e.g., DeLong's test) to compare the reported AUCs. Therefore, the added value of these complex models over simpler approaches is not demonstrated statistically.

While Example #5 compares the complex model (Random Forest) to a classical model (Logistic Regression) and a simple baseline (No Information Rate), it fails because it does not use any appropriate statistical tests (like DeLong's test or significance testing against the No Information Rate) to determine if the observed performance differences (in accuracy and AUC) are statistically significant. Simply reporting numerically higher metrics is insufficient; statistical validation is required.

### Recommendations for appropriate scoring
It is important to distinguish this requirement from general statistical analyses presented in the study. This item specifically assesses whether the study compares the proposed complex model against a simple or baseline model to determine whether the added complexity is justified.

If only a simple model is used, there should be at least a comparison with a no-information case.
A study that lacks a formal statistical method (e.g., DeLong’s test) for comparing model performance should not receive a positive score for this item.

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Romeo V, Cuocolo R, Apolito R, et al (2021) Clinical value of radiomics and machine learning in breast ultrasound: a multicenter study for differential diagnosis of benign and malignant lesions. Eur Radiol 31:9511–9519. https://doi.org/10.1007/s00330-021-08009-2
3. 	Yin P, Zhong J, Liu Y, et al (2023) Clinical-radiomics models based on plain X-rays for prediction of lung metastasis in patients with osteosarcoma. BMC Med Imaging 23:40. https://doi.org/10.1186/s12880-023-00991-x
4. 	Mylona E, Zaridis DI, Kalantzopoulos CΝ, et al (2024) Optimizing radiomics for prostate cancer diagnosis: feature selection strategies, machine learning classifiers, and MRI sequences. Insights Imaging 15:265. https://doi.org/10.1186/s13244-024-01783-9

[Previous: Item #24](https://radiomic.github.io/METRICS-E3/docs/Metrics%20and%20Comparison%20(Item%2020-25)/Item%2024.html){: .btn .btn-purple  .mr-5  }
[Next: Item #26](https://radiomic.github.io/METRICS-E3/docs/Testing%20(Item%2026-27)/Item%2026.html){: .btn .btn-purple   }
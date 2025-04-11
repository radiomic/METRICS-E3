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
> **Example #1:** “After generating the best threshold for the predicted probabilities for LASSO and PLS, the confusion matrix and metric analysis have shown only a slightly higher accuracy (0.80 and 0.81) than the no information rate (0.736, p = 0.011 and 0.736, p = 0.005) in the validation set, respectively.” [2] (licensed under CC BY)

> **Example #2:** “Linear regression (LR), Random Forest (RF), and convolutional neural network (CNN) algorithms were used to predict the Child-Pugh class. […] The measured accuracies were tested against the no-information rate, a classifier that assigns the most prevalent class to all samples. […] Significantly better accuracies for the prediction of Child-Pugh classes versus no-information rate were found for CNN and ERs (p ≤ 0.034), not for LR and RF (p ≥ 0.384).” [3] (licensed under CC BY)

> **Example #3:** “The final selected features were utilized for modelling with five mainstream classifiers, including logistic regression (LR), K-nearest neighbours (KNN), support vector machine (SVM), random forest (RF) and GaussianNB (Gnb). […] DeLong’s test was utilized for comparisons of AUCs. A p value < 0.05 indicates a significant difference.” [4] (licensed under CC BY)

“MPGTs vs. PA […] Analysis by Delong’s test showed that the AUC of the RF model was the highest but was significantly higher than that of the Gnb model only (p=0.021), with no significant differences compared to those of the other three models (p>0.05).” [4] (licensed under CC BY)

“MPGTs vs. WT […] Analysis by Delong’s test showed that the AUC of the SVM model was significantly better than that of the LR model (p=0.022) or Gnb model (p=0.010), but there was no significant difference compared to the AUCs of the RF and KNN models (p>0.05).” [4] (licensed under CC BY)

### Hypothetical negative examples
> **Example #4:** ...To evaluate the optimal approach for classifying glioma grade, we implemented and compared three distinct deep learning architectures: a standard 3D Convolutional Neural Network (3D-CNN), a Residual Network (ResNet) adaptation, and a Vision Transformer (ViT) model tailored for volumetric medical data. All models were trained on our institutional dataset (n=450) and evaluated on an external validation cohort (n=110). Performance was assessed using the Area Under the Receiver Operating Characteristic Curve (AUC). The ViT model achieved the highest AUC of 0.92, followed by the ResNet (AUC = 0.90) and the standard 3D-CNN (AUC = 0.88). While the ViT demonstrated the best performance numerically, further studies are needed to confirm its clinical utility...

> **Example #5:** ...We developed a Random Forest (RF) model utilizing 85 radiomic features extracted from pre-treatment CT scans to predict patient response to immunotherapy. For benchmarking, we also trained a Logistic Regression (LR) model using the same feature set. The models were evaluated on an independent test set (n=95). The RF model achieved an accuracy of 76% and an AUC of 0.81. The LR model showed an accuracy of 72% and an AUC of 0.77. The No Information Rate (predicting the majority class 'non-responder') yielded an accuracy of 65%. Our results suggest the RF model provides better predictive performance than the simpler LR model and baseline chance...

### Importance of the item
Comparing radiomic or deep learning models to simple or classical statistical models is essential to demonstrate their true added value. Without such comparisons, it becomes unclear whether complex techniques offer any meaningful advantage over basic approaches. Simple models, such as logistic regression or Zero Rules classifiers, often perform surprisingly well, particularly in small datasets. By applying proper statistical tests, such as DeLong’s test or Net Reclassification Index, researchers can objectively assess performance gains, ensuring that increased model complexity is scientifically justified rather than arbitrarily applied.

### Specifics about the positive examples
Examples #1 and #2 include comparisons with the no-information rate, supported by formal statistical testing. Example #3 compares multiple algorithms, ranging from basic to complex, and provides statistical comparisons to evaluate their relative performance.

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
2. 	Gorodetski B, Becker PH, Baur ADJ, et al (2022) Inferring FDG-PET-positivity of lymph node metastases in proven lung cancer from contrast-enhanced CT using radiomics and machine learning. European Radiology Experimental 6:44. https://doi.org/10.1186/s41747-022-00296-8
3. 	Thüring J, Rippel O, Haarburger C, et al (2020) Multiphase CT-based prediction of Child-Pugh classification: a machine learning approach. European Radiology Experimental 4:20. https://doi.org/10.1186/s41747-020-00148-3
4. 	Lu Y, Liu H, Liu Q, et al (2023) CT-based radiomics with various classifiers for histological differentiation of parotid gland tumors. Front Oncol 13:. https://doi.org/10.3389/fonc.2023.1118351

[Back](https://radiomic.github.io/METRICS-E3/){: .btn .btn-purple  .mr-5  }
[Next](https://radiomic.github.io/METRICS-E3/docs/Study%20Design%20(Item%201-3)/Item%202.html){: .btn .btn-purple   }
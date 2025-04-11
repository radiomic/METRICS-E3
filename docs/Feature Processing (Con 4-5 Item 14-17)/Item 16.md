---
title: Item#16
layout: home
parent: 5. Feature Processing
nav_order: 5
---

### Item #16
“Appropriateness of dimensionality compared to data size.” [1]  (licensed under CC BY)

### Explanation
“Whether the number of instances and features in the final training data set is appropriate according to the research question and modeling algorithm. This should be demonstrated by statistical means, empirically through consistency of performance in validation and testing, or based on previous evidence in the literature.” [1]  (licensed under CC BY)

“This item is conditional. It is applicable only for the studies having tabular data (i.e., numeric radiomic features in a tabulated format, which is usually seen in hand-crafted and some deep learning-based studies as deep features).” [1]  (licensed under CC BY)

### Positive examples from the literature 
> **Example #1:** “According to multivariable logistic regression, age, gender, and the mean CT value were selected to build clinical-radiographic-based model. After LASSO and the stepwise logistic regression analysis were conducted, three radiomics features were ultimately selected to build a radiomics-feature-based model. These features included the Log.5.0_glszm_SmallAreaHighGrayLevelEmphasis, wavelet.LHL_glcm_MCC, and wavelet.LLL_glcm_SumAverage.” [2] (licensed under CC BY)
>
> Also see **Table 1**.
> 
> **Table 1.** “Demographic characteristics” (cropped; licensed under CC BY)
>![Tab1](/METRICS-E3/figs/Item16 T1.png) 
>

> **Example #2:** “For maximizing the discrimination of radiomics algorithm, the machine-learning classifiers of logistic regression, decision tree, random forest, and support vector machine (SVM) were implemented to model construction, respectively. In this study, SVM showed the best performance in terms of discrimination and was finally selected **[Table 2]**.” [3] (licensed under CC BY)
>
> “A total of 18 optimal feature subsets were selected, including 1 shape feature, 13 texture features, and 4 first-order statistics features.” [3] (licensed under CC BY)
>
> **Table 2.** “The classification results of ablation analyses on training, internal, and external test cohort” [3] (licensed under CC BY)
>
>![Tab2](/METRICS-E3/figs/Item16 T2.png) 

### Hypothetical negative examples 
> **Example #3:** The radiomics signature was developed using logistic regression and specifically by LASSO, which selected 25 features. The final training set consisted of 80 patients, 30 of whom experienced disease progression.

> **Example #4:** We employed a random forest classifier using 15 radiomic features extracted from MR images. The final training set consisted of 120 patients, 60 of whom experienced disease progression. The classifier achieved very high performance on the training cohort with an AUC of 0.98 (95% CI: 0.96–1.00), but showed substantially reduced performance in both the internal validation cohort (AUC: 0.85; 95% CI: 0.78–0.90) and the external testing cohort (AUC: 0.79; 95% CI: 0.74–0.83).

> **Example #5:** We conducted sample size estimation with a significance level (a) of 0.05 and power of 0.80. Consequently, a sample size of 110 patients was obtained.

> **Example #6:** To determine an appropriate sample size, we performed a power calculation based on the expected area under the ROC curve (AUC). Assuming an anticipated AUC of 0.80 with an alpha error of 0.05 and 80% power, the minimum required sample size was estimated to be 50 patients per group.

### Importance of the item
Dealing with high-dimensional data introduces the curse of dimensionality in radiomics, which limits the generalization ability of models and necessitates a large number of samples to be addressed [4]. Unbalance between sample size and feature dimensionality introduces a risk of either over- or underfitting, respectively translating into a performance drop from training to testing and underperformance in training for failing to capture the problem complexity. While some “rules of thumb” have been proposed in the literature to define the number of required samples in function of the feature’s dimensionality (e.g., 10 samples for every included feature), there is no unequivocal answers to this complex issue which should be faced on a per case base [5]. This could be done by means of statistical tools that are available to provide reliable estimates of the required sample size [6]. An indirect proof of an adequate sample is provided by the stability of the models’ performance on independent unseen data (i.e., of good generalizability).

### Specifics about the positive examples
In Example #1, the study deemed dimensionality adequate based on the logistic regression “rule of thumb.” Specifically, the training cohort consisted of 232 patients, 60 of whom belonged to the minority class. From this 1:10 minority-to-parameter ratio, the study identified 6 total features (3 clinical and 3 radiomics), making the dimensionality appropriate not only for the overall training cohort but also for the minority class. Table 1 provides detailed information regarding the number of instances within each class.

In Example #2, dimensionality was evaluated by examining the model’s fit rather than using the 1:10 rule, since the best-performing classifier was a support vector machine (SVM). The primary assessment came from comparing 95% confidence intervals for the area under the curve (AUC) in both training and testing cohorts (internal and external). While the mean AUC was slightly higher in the internal testing cohort and slightly lower in the external testing cohort, the substantial overlap in confidence intervals indicates a satisfactory model fit, which may indicate appropriateness of dimensionality.

### Specifics about the negative examples
In Example #3, the algorithm selected 25 features for logistic regression, but there were only 30 patients experiencing disease progression. According to the logistic regression rule of thumb (ideally, 10 patients per feature from the minority class), making this sample clearly inadequate. 

In Example #4, despite a seemingly sufficient sample size, the significant performance drop from training to validation and external testing cohorts (indicated by distinct confidence intervals) strongly suggests model overfitting due to inappropriate dimensionality. 

Examples #5 and #6 used simplistic sample-size calculations based solely on statistical power and anticipated AUC without explicitly considering feature dimensionality, ignoring critical issues related to radiomic analyses and resulting in insufficient justification for their sample sizes.

### Recommendations for appropriate scoring
When evaluating the appropriateness of dimensionality, it is crucial to use methods aligned with the specific algorithm under study. For logistic regression, traditional rules of thumb can be applied, or more advanced techniques such as those proposed by Riley et al. may be adopted [7–10]. 

In the case of more complex algorithms, the model’s fitting status can serve as an indirect gauge of dimensionality. However, it is vital to assess this status using uncertainty measures (e.g., 95% confidence intervals) rather than relying solely on point estimates like the mean. 

For complex models — meaning models other than logistic regression — the rule of thumb of 1:10 for the minority class can also be used as an partial check to assess whether the required sample size would fall short for simpler models. If the sample size is insufficient for simpler models, this would suggest that the dimensionality is also likely inappropriate relative to the data size for complex models. However, this rule of thumb should not be solely relied upon to fully determine whether the criteria are satisfied.

Finally, simple sample-size calculations that do not explicitly account for dimensionality—such as those based solely on measures like the AUC—are insufficient to fully address this concern.

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Feng H, Shi G, Xu Q, et al (2023) Radiomics-based analysis of CT imaging for the preoperative prediction of invasiveness in pure ground-glass nodule lung adenocarcinomas. Insights Imaging 14:24. https://doi.org/10.1186/s13244-022-01363-9
3. 	Yu Y, Yang T, Ma P, et al (2025) Determining the status of tertiary lymphoid structures in invasive pulmonary adenocarcinoma based on chest CT radiomic features. Insights into Imaging 16:28. https://doi.org/10.1186/s13244-025-01906-w
4. 	Kuo MD, Jamshidi N (2014) Behind the Numbers: Decoding Molecular Phenotypes with Radiogenomics—Guiding Principles and Technical Considerations. Radiology 270:320–325. https://doi.org/10.1148/radiol.13132195
5. 	van Timmeren JE, Cester D, Tanadini-Lang S, et al (2020) Radiomics in medical imaging—“how-to” guide and critical reflection. Insights into Imaging 11:91. https://doi.org/10.1186/s13244-020-00887-2
6. 	Riley RD, Snell KI, Ensor J, et al (2019) Minimum sample size for developing a multivariable prediction model: PART II - binary and time-to-event outcomes. Statistics in Medicine 38:1276–1296. https://doi.org/10.1002/sim.7992
7. 	Zhong J, Liu X, Lu J, et al (2025) Overlooked and underpowered: a meta-research addressing sample size in radiomics prediction models for binary outcomes. Eur Radiol 35:1146–1156. https://doi.org/10.1007/s00330-024-11331-0
8. 	Pate A, Riley RD, Collins GS, et al (2023) Minimum sample size for developing a multivariable prediction model using multinomial logistic regression. Stat Methods Med Res 32:555–571. https://doi.org/10.1177/09622802231151220
9. 	Riley RD, Debray TPA, Collins GS, et al (2021) Minimum sample size for external validation of a clinical prediction model with a binary outcome. Stat Med 40:4230–4251. https://doi.org/10.1002/sim.9025
10. 	Riley RD, Snell KI, Ensor J, et al (2019) Minimum sample size for developing a multivariable prediction model: PART II - binary and time-to-event outcomes. Stat Med 38:1276–1296. https://doi.org/10.1002/sim.7992

[Back](https://radiomic.github.io/METRICS-E3/docs/Feature%20Processing%20(Con%204-5%20Item%2014-17)/Item%2015.html){: .btn .btn-purple  .mr-5  }
[Next](https://radiomic.github.io/METRICS-E3/docs/Feature%20Processing%20(Con%204-5%20Item%2014-17)/Item%2017.html){: .btn .btn-purple   }


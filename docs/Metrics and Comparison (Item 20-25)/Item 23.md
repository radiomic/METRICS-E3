---
title: Item#23
layout: home
parent: 7. Metrics and Comparison
nav_order: 4
---

### Item #23 
“Use of uni-parametric imaging or proof of its inferiority” [1]  (licensed under CC BY)

### Explanation
“Use of a single imaging set (such as a single MRI sequence rather than multiple, or a single phase in a dynamic contrast-enhanced scan) should be preferred, as multi-parametric imaging may unnecessarily increase data dimensionality and risk of overfitting. Therefore, in the case of multi-parametric studies, uni-parametric evaluations should also be performed to justify the need for a multi-parametric approach by formally comparing their performance (e.g., DeLong’s or McNemar’s tests). This item is also intended to reward studies that experimentally justify the use of more complex models compared to simpler alternatives, in regard to input data type.” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “The segmentation of hypoxia on the 18F-FMISO-PET image acquired before treatment (HSV_W0) was transferred to all co-registered PET series. The 130 radiomic features were computed for each 18F-FMISO time-point using an open-source code based on MATLAB® (The MathWorks Inc., Natick, MA, USA).” [2] (licensed under CC BY)

> **Example #2:** “The imaging protocol included an unenhanced phase, followed by the injection of a non-ionic contrast agent (Ultravist 350/370, Bayer Healthcare) at a specific dose (1.2 mL/kg) and flow rate (3.5–5.0 mL/s). A saline flush of 30–40 mL at the same injection rate was administered. The arterial phase scanning was initiated 10–15 s after reaching a trigger threshold (100 HU) in the abdominal aorta, and the portal venous phase scanning was conducted 30–35 s after the end of the arterial phase.” […] (1) Tumor segmentation: Radiologist 1 performed three-dimensional volume of interest (3D-VOI) segmentation along the tumor margin excluding cysts, necrosis, blood vessels, and lymph nodes in side tumor on axial portal venous phase CT images using ITK-SNAP software (version 3.8.0, http://www.itksnap.org/). We did not choose the arterial phase because the tumor boundary was more distinct and evident in the portal venous phase, which contribute to tumor segmentation. […] A total of 1051 radiomics features were initially extracted from the 3D segmented VOI based on the portal venous phase. The analysis of variance performs initial feature screening to reduce the complexity of LASSO feature screening. 10 features with nonzero coefficients were selected through lasso regression. Figure 3 illustrates the selection process of the LASSO model and the visualization of features. Finally, to prevent overfitting due to an excessive number of features, PCA was performed to reduce dimensionality, and features were finally reduced to 6.” [3] (licensed under CC BY)

> **Example #3:** “Separate models were trained using either radiomic features from a single image type (single-modality models: PSMA-PET, T1w, T2w, ADC) or combined from PET and each MR sequence (double-modality models: PSMAPET+T1w, PSMA-PET+T2w, PSMA-PET+ ADC). The use of more than two image types — such as PET and several MR sequences — was not implemented for two reasons: first, the exponentially higher computing time required to train a model with all the features and combined hyperparameters from many modalities; second, the relative low outcome changes obtained from adding extra modalities in previous experiences. […] Results from the baseline models, PET-only radiomics, each MR-modality (T1w, T2w, ADC) radiomics only, and combined PET+MR radiomics were compared using Student’s t-test. […] All radiomic models outperformed the baseline models. The best-performing (mean ± stdv [%]) single-modality model was the ADC model (76 ± 6%), although not significantly better (p > 0.05) than other single-modality models (T1w: 72 ± 3%, T2w: 73 ± 2%; PET: 75 ± 5%). The overall best-performing model combined PET + ADC radiomics (82 ± 5%). It significantly outperformed most other double-modality (PET + T1w: 74 ± 5%, p = 0.026; PET + T2w: 71 ± 4%, p = 0.003) and single-modality models (PET: p = 0.042; T1w: p = 0.002; T2w: p = 0.003), except the ADC-only model (p = 0.138). In this initial cohort, the PET + ADC model outperformed bGS overall (82.5% vs 72.4%) in the prediction of psGS.” [4] (licensed under CC BY)

> **Example #4:** “Eight radiomic models (Models 1–8) were developed for TNBC identification, using the following combinations of quantitative parameters and radiomic features: quantitative parameters alone (Model 1); radiomic features extracted from ADC (Model 2), DCE (Model 3), PET (Model 4) and T2-weighted (Model 5) images; combinations of radiomic features extracted from different 18F-FDG PET/MR images, namely DCE-MRI and ADC (Model 6), and DCE-MRI, ADC, and PET (Model 7); and quantitative parameters combined with radiomic features (Model 8). […] McNemar’s test was used to assess differences in terms of diagnostic performance among the different radiomics models. p values ≤ 0.05 were considered statistically significant.” [5] (licensed under CC BY)

### Hypothetical negative examples
> **Example #5:** Radiomic features were extracted from co-registered T1-weighted contrast-enhanced (T1CE) and FLAIR MRI sequences. The 215 features (105 from T1CE, 110 from FLAIR) were concatenated and subsequently reduced using principal component analysis prior to input into a support vector machine classifier to predict tumor grade

> **Example #6:** We developed predictive models using features from baseline CT (Model A) and baseline FDG-PET (Model B), as well as a combined model using features from both CT and PET (Model C). Model A achieved AUC=0.78, Model B achieved AUC=0.81, and Model C achieved AUC=0.84. We therefore utilized Model C for further analysis as it demonstrated the highest AUC.

### Importance of the item
This item directly addresses the 'curse of dimensionality,' where incorporating more data types or features to train a model with limited examples often leads to suboptimal performance [6, 7]. The more data dimensions a model has, the more complex and challenging the feature selection process becomes, increasing the risk of overfitting and reduced generalizability. Simpler models should also be favoured for their improved explainability and reduced risk of redundant information [8].

Data sparsity is a significant issue in radiomics, as patient datasets are typically small [9]. Requiring multiple imaging modalities further narrows the pool of eligible training data, exacerbating this challenge. Therefore, models should be trained on the largest possible sample size to ensure robust and reliable results, prioritizing data volume over the inclusion of multiple imaging sequences. The inclusion of additional sequences or modalities should be justified only if their contribution to the model’s performance is demonstrated through formal statistical comparisons, such as DeLong’s or McNemar’s tests.

### Specifics about the positive examples
Examples #1 and #2 are good examples because they extracted radiomics features only from a single imaging set. Precisely, Example #1 only focused on 18F-FMISO-PET for hypoxia monitoring, while Example #2 only used portal venous phase CT images to characterize pancreatic ductal adenocarcinoma. Conversely, Examples #3 and #4 investigated multimodal imaging sets, but they also performed uni-parametric evaluations that were compared to the more complex models via appropriate tests such as Student’s t-test and McNemar’s test. It is important to note that using multi-parametric imaging sets is not inherently wrong. However, it requires more careful feature selection and additional analysis to demonstrate the added value of integrating different image types.

### Specifics about the negative examples
Example #5 uses multi-parametric data (T1CE and FLAIR) but fails because it immediately combines the features without first evaluating or reporting the performance of uni-parametric models (T1CE-only or FLAIR-only). Therefore, the need for the multi-parametric approach is not justified. Example #6 evaluates both uni-parametric (CT-only, PET-only) and multi-parametric (CT+PET) models. However, it fails because it justifies the use of the combined model based solely on its numerically higher AUC, without performing a formal statistical comparison (e.g., DeLong's test) to demonstrate that the performance improvement over the uni-parametric models is statistically significant.

### Recommendations for appropriate scoring 
Studies that extract radiomics features from a single imaging set (such as a single MRI sequence or a single radiotracer in PET studies) should be awarded a point from the METRICS. 

Studies exploring multi-parametric or multi-modal radiomics features receive a point only if they also conduct uni-parametric evaluations and use appropriate statistical tests to compare performance against the more complex models.

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Carles M, Fechter T, Grosu AL, et al (2021) 18F-FMISO-PET Hypoxia Monitoring for Head-and-Neck Cancer Patients: Radiomics Analyses Predict the Outcome of Chemo-Radiotherapy. Cancers 13:3449. https://doi.org/10.3390/cancers13143449
3. 	Liao H, Yuan J, Liu C, et al (2023) Feasibility and effectiveness of automatic deep learning network and radiomics models for differentiating tumor stroma ratio in pancreatic ductal adenocarcinoma. Insights Imaging 14:223. https://doi.org/10.1186/s13244-023-01553-z
4. 	Solari EL, Gafita A, Schachoff S, et al (2022) The added value of PSMA PET/MR radiomics for prostate cancer staging. Eur J Nucl Med Mol Imaging 49:527–538. https://doi.org/10.1007/s00259-021-05430-z
5. 	Romeo V, Kapetas P, Clauser P, et al (2022) A Simultaneous Multiparametric 18F-FDG PET/MRI Radiomics Model for the Diagnosis of Triple Negative Breast Cancer. Cancers 14:3944. https://doi.org/10.3390/cancers14163944
6. 	Verleysen M, François D (2005) The Curse of Dimensionality in Data Mining and Time Series Prediction. In: Cabestany J, Prieto A, Sandoval F (eds) Computational Intelligence and Bioinspired Systems. Springer Berlin Heidelberg, Berlin, Heidelberg, pp 758–770
7. 	Crespo Márquez A (2022) The Curse of Dimensionality. In: Digital Maintenance Management. Springer International Publishing, Cham, pp 67–86
8. 	Escobar T, Vauclin S, Orlhac F, et al (2022) Voxel‐wise supervised analysis of tumors with multimodal engineered features to highlight interpretable biological patterns. Medical Physics 49:3816–3829. https://doi.org/10.1002/mp.15603
9. 	Ghezzo S, Bezzi C, Presotto L, et al (2022) State of the art of radiomic analysis in the clinical management of prostate cancer: A systematic review. Critical Reviews in Oncology/Hematology 169:103544. https://doi.org/10.1016/j.critrevonc.2021.103544

[Previous: Item #22](https://radiomic.github.io/METRICS-E3/docs/Metrics%20and%20Comparison%20(Item%2020-25)/Item%2022.html){: .btn .btn-purple  .mr-5  }
[Next: Item #24](https://radiomic.github.io/METRICS-E3/docs/Metrics%20and%20Comparison%20(Item%2020-25)/Item%2024.html){: .btn .btn-purple   }

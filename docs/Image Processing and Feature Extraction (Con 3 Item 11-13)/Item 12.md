---
title: Item#12
layout: home
parent: 4. Image Processing and Feature Extraction
nav_order: 3
---

### Item #12
“Use of standardized feature extraction software” [1]  (licensed under CC BY)

### Explanation
“Whether a standardized software (e.g., compliant with IBSI) was used for feature extraction, including information on the version number.” [1]  (licensed under CC BY)
“This item is conditional. It is applicable only for studies with hand-crafted radiomic features. In the case of DL studies, the exclusion of this item from scoring will not affect the final score in the percentage scale.” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “Feature extraction was performed using the open-source package pyradiomics v3.0 in compliance with Image Biomarker Standardization Initiative−IBSI standards.” [2] (licensed under CC BY)

> **Example #2:** “258 radiomics features were extracted using the IBSI-conform and validated MITK phenotyping toolbox (version 2022.4, German Cancer Research Center, Heidelberg, Germany).” [3] (licensed under CC BY)

> **Example #3:** “Radiomic features were extracted using the LIFEx platform version 6.1 (IMIV/CEA, Orsay, France) from axial PET, low-dose unenhanced CT (acquired as part of the PET/CT), axial fat saturated and contrast-enhanced T1-w and T2-w RP-MR Digital Imaging and Communications in Medicine (DICOM) images that had been archived in PACS.” [4] (licensed under CC BY)

> **Example #4:** “75 Radiomics features were extracted within each segmented liver lesion by employing Pyradiomics (version 3.0.1) in Python.” [5] (licensed under CC BY)

### Hypothetical negative examples
> **Example #5:** “Radiomic features were extracted from segmented tumor regions using an in-house script developed in MATLAB.”

> **Example #6:** “Feature extraction was conducted using various image processing tools available in Python.”

> **Example #7:** “Feature extraction was conducted using PyRadiomics.”

### Importance of the item
Feature extraction is a fundamental step of the radiomic workflow [6]. Employing different extraction methods could significantly affect the reproducibility of radiomic studies and, in hand-crafted radiomics, this occurs especially when no details on the software used are provided or when in-house developed tools are employed [7]. The Image Biomarker Standardization Initiative (IBSI) has defined a set of standardized radiomic features and provided guidelines for verifying and calibrating the feature extraction software programs [8]. The employment of IBSI-compliant software may reduce inter-study variability, improving the generalizability of radiomic models [9, 10]. Additionally, reporting the software versions in the manuscript is fundamental for reproducibility, as even minor updates can impact the reliability of feature extraction [9].

### Specifics about the positive examples
All the reported examples include a detailed description of the software employed for the feature extraction, including name, version, and direct reference to software documentation. The three software reported in the examples – Pyradiomics and LifeX - are commonly used for traditional radiomic features extraction and they claim to be IBSI-compliant, as also explicitly stated in Examples #1 and #2 with inclusion of the related reference to IBSI paper.

Example #4 further specifies the use of Python for PyRadiomics (open-source package) in the Methods section, providing the same information also in the caption of the second figure included in the manuscript where the entire radiomic workflow is depicted.  Differently, a similar information is not required for Example #3 due to the standalone nature of the LIFEx software that does not require integration with other tools.

### Specifics about the negative examples
Example #5 does not specify the use of a standardized or IBSI-compliant tool, relying instead on an in-house MATLAB script, which may not be validated or reproducible. Example #6 is vague, failing to identify the specific software or its compliance with standardization guidelines, making it unclear whether the methods used are consistent with best practices. Example #7, while mentioning PyRadiomics, does not include the version number, which is critical for reproducibility since different versions may yield different results.

### Recommendations for appropriate scoring
Authors are encouraged to provide a detailed description of the software used for feature extraction to ensure transparency and reproducibility of the radiomic study. The required software details should include name, version, and evidence of standardization, such as references to IBSI compliance. A list of IBSI compliant tools can be accessed at https://theibsi.github.io/implementations/. Reporting the environment or the dependent library versions is advised, but not mandatory. Furthermore, providing references or links to the software documentation can further support the alignment with standardization guidelines.

Studies that lack these fundamental software details, fail to provide evidence of standardization, or rely on in-house or non-compliant tools should not receive points under the METRICS. 

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Bodalal Z, Hong EK, Trebeschi S, et al (2024) Non-invasive CT radiomic biomarkers predict microsatellite stability status in colorectal cancer: a multicenter validation study. European Radiology Experimental 8:98. https://doi.org/10.1186/s41747-024-00484-8
3. 	Wennmann M, Rotkopf LT, Bauer F, et al (2025) REPRODUCIBLE RADIOMICS FEATURES FROM MULTI‐MRI‐SCANNER TEST–RETEST‐STUDY: INFLUENCE ON PERFORMANCE AND GENERALIZABILITY OF MODELS. Magnetic Resonance Imaging 61:676–686. https://doi.org/10.1002/jmri.29442
4. 	Kulanthaivelu R, Kohan A, Hinzpeter R, et al (2022) Prognostic value of PET/CT and MR-based baseline radiomics among patients with non-metastatic nasopharyngeal carcinoma. Front Oncol 12:952763. https://doi.org/10.3389/fonc.2022.952763
5. 	Pietsch FL, Haag F, Ayx I, et al (2024) Textural heterogeneity of liver lesions in CT imaging - comparison of colorectal and pancreatic metastases. Abdom Radiol 49:4295–4306. https://doi.org/10.1007/s00261-024-04511-5
6. 	Lambin P, Rios-Velazquez E, Leijenaar R, et al (2012) Radiomics: Extracting more information from medical images using advanced feature analysis. European Journal of Cancer 48:441–446. https://doi.org/10.1016/j.ejca.2011.11.036
7. 	Song J, Yin Y, Wang H, et al (2020) A review of original articles published in the emerging field of radiomics. European Journal of Radiology 127:108991. https://doi.org/10.1016/j.ejrad.2020.108991
8. 	Zwanenburg A, Vallières M, Abdalah MA, et al (2020) The Image Biomarker Standardization Initiative: Standardized Quantitative Radiomics for High-Throughput Image-based Phenotyping. Radiology 295:328–338. https://doi.org/10.1148/radiol.2020191145
9. 	Fornacon-Wood I, Mistry H, Ackermann CJ, et al (2020) Reliability and prognostic value of radiomic features are highly dependent on choice of feature extraction platform. Eur Radiol 30:6241–6250. https://doi.org/10.1007/s00330-020-06957-9
10. 	Bortolotto C, Pinto A, Brero F, et al (2024) CT and MRI radiomic features of lung cancer (NSCLC): comparison and software consistency. Eur Radiol Exp 8:71. https://doi.org/10.1186/s41747-024-00468-8

[Back](https://radiomic.github.io/METRICS-E3/docs/Image%20Processing%20and%20Feature%20Extraction%20(Con%203%20Item%2011-13)/Item%2011.html){: .btn .btn-purple  .mr-5  }
[Next](https://radiomic.github.io/METRICS-E3/docs/Image%20Processing%20and%20Feature%20Extraction%20(Con%203%20Item%2011-13)/Item%2013.html){: .btn .btn-purple   }


---
title: Item#28
layout: home
parent: 9. Open Science
nav_order: 1
---

Item #28
“Data availability” [1]  (licensed under CC BY)
Explanation
“Whether any imaging, segmentation, clinical, or radiomics analysis data is shared with the public.” [1] (licensed under CC BY)
Positive examples from the literature
Example #1: “Imaging and clinical research data are publicly available and can be found at https://xnat.bmia.nl/data/projects/worc and are described in detail in https://doi.org/10.1101/2021.08.19.21262238.” [2] (licensed under CC BY)
Example #2: “The data generated and analyzed during this study are described in the following data record: https://doi.org/10.6084/m9.figshare.12912191. The datasets are as follows: the original acquired and derived MRI DICOM data, under the title “I-SPY 2 MRI Collection”, and an Excel file called “Multi-feature MRI NACT Data.xlsx”. These will be deposited and be publicly available in NCI The Cancer Imaging Archive (TCIA): https://www.cancerimagingarchive.net/.” [3] (licensed under CC BY)
Example #3: ““The data and the R code that support the findings of this study are available at https://github.com/harveerar/SciRepEndometrial2020.” [4] (licensed under CC BY)
Example #4: “The corresponding manually generated lesion segmentations are publicly available (https://github.com/rcuocolo/PROSTATEx_masks).” [5] (licensed under CC BY)
Example #5: “The imaging and clinical research data for part of this study (data set A) have been made publicly available: https://doi.org/10.1101/2021.08.19.21262238.” [6] (licensed under CC BY)
Hypothetical negative examples
Example #6: The datasets generated and/or analyzed during the current study are available from the corresponding author on reasonable request.
Example #7: Due to institutional policies and patient privacy regulations regarding the sensitive nature of the clinical data, the datasets supporting the conclusions of this article are not publicly available.
Example #8: The radiomic features extracted for this study are listed in Supplementary Table S3. Further underlying data may be shared pending approval from the Institutional Review Board and data use agreements.
Example #9:  The imaging and segmentation data supporting the findings of this study have been deposited in the [Name of Repository, e.g., University Secure Archive] repository ([Hypothetical Link/Identifier]). A download code is required for access and can be provided by the corresponding author upon reasonable request and verification.
Importance of the item 
Data availability is a cornerstone of open science practices at the base of reproducibility of radiological research [7–9]. The FAIR principles (Findable, Accessible, Interoperable, Reusable) provide a framework to improve data accessibility and reusability [10] These principles are particularly important in radiomics because, despite an increasing number of models publications, clinical implementation is still limited [11]. A major barrier is the lack of data sharing that does not allow model validation into independent datasets [9], limiting the generalizability of the developed models. As a result, some attempts have been made to promote this process, such as the RadiomicsHub [12]- a repository of radiomics features extracted from public imaging datasets – or RadBase [9] – a searchable radiomic research database. These initiatives of data sharing in radiomics are fundamental and could pave the way to more transparent protocols and favor a progressive widespread clinical adoption.
Specifics about the positive examples
The included examples demonstrate different possibilities of data sharing that range from single databases of extracted radiomic features, as in Examples #3, to imaging with related segmentations in Example #1 and Example #4 up to the availability of more comprehensive clinical and radiological datasets of Example #2. Moreover, Examples #1 and #2 relies on data publications on widely recognized data repositories, i.e. ZENODO [13], XNAT [14] and The Cancer Imaging Archive [15] respectively. However, Example #2 lacks a direct link to the public available dataset, requiring users to find it directly on the external repository, which slightly reduce accessibility. In Example #3, authors included radiomic feature data as well as clinical data. Example #4 provides the segmentation dataset. Example #5 refers to the source article of the WORC database.
Specifics about the negative examples
In Example #6, data access is conditional ("on reasonable request") and mediated by the author, not directly and publicly available. This creates barriers and uncertainty, contradicting open data principles. Example #7 explicitly states that the data is not publicly available, directly failing the requirement for public data sharing, even if reasons are provided. In Example #8, while some derived information (feature list) might be present, the underlying analyzable data requires conditional access (approvals, agreements). This restricted access does not meet the standard for open, public data availability required for replication. Example #9 is negative because access to the data in the repository is restricted by a non-public code obtainable only via author request and verification, making it not openly and publicly accessible.
Recommendations for appropriate scoring
The requirements for point assignments are quite broad, allowing authors to decide to share clinical, radiological or radiomics data, according also to privacy regulations. For appropriate scoring, the completeness, accessibility, and usability of the shared data must be assessed, and the use of public repositories, direct links, or proper documentation is essential. 
Studies that declare data availability but fail to provide direct or indirect access should not be awarded points. Furthermore, terms like "data available upon request" or requiring excessive permissions should not qualify as open sharing, as they often affect reproducibility and thus not gain point from the METRICS. 
Points should be awarded only if datasets are fully accessible with sufficient documentation to allow reanalysis and replication. 
It is essential to provide the labels of radiomic features when sharing radiomic feature data. Simply giving radiomic values without linking them to a specific class or outcome should not be considered adequate for meeting this item.
References
1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Starmans MPA, Timbergen MJM, Vos M, et al (2022) Differential Diagnosis and Molecular Stratification of Gastrointestinal Stromal Tumors on CT Images Using a Radiomics Approach. J Digit Imaging 35:127–136. https://doi.org/10.1007/s10278-022-00590-2
3. 	Li W, Newitt DC, Gibbs J, et al (2020) Predicting breast cancer response to neoadjuvant treatment using multi-feature MRI: results from the I-SPY 2 TRIAL. npj Breast Cancer 6:63. https://doi.org/10.1038/s41523-020-00203-7
4. 	Veeraraghavan H, Friedman CF, DeLair DF, et al (2020) Machine learning-based prediction of microsatellite instability and high tumor mutation burden from contrast-enhanced computed tomography in endometrial cancers. Sci Rep 10:17769. https://doi.org/10.1038/s41598-020-72475-9
5. 	Mylona E, Zaridis DI, Kalantzopoulos CΝ, et al (2024) Optimizing radiomics for prostate cancer diagnosis: feature selection strategies, machine learning classifiers, and MRI sequences. Insights into Imaging 15:265. https://doi.org/10.1186/s13244-024-01783-9
6. 	Starmans MPA, Miclea RL, Vilgrain V, et al (2024) Automated Assessment of T2-Weighted MRI to Differentiate Malignant and Benign Primary Solid Liver Lesions in Noncirrhotic Livers Using Radiomics. Academic Radiology 31:870–879. https://doi.org/10.1016/j.acra.2023.07.024
7. 	Sardanelli F, Alì M, Hunink MG, et al (2018) To share or not to share? Expected pros and cons of data sharing in radiological research. Eur Radiol 28:2328–2335. https://doi.org/10.1007/s00330-017-5165-5
8. 	Kocak B, Yardimci AH, Yuzkan S, et al (2023) Transparency in artificial intelligence research: a systematic review of availability items related to open science in radiology and nuclear medicine. Academic Radiology 30:2254–2266. https://doi.org/10.1016/j.acra.2022.11.030
9. 	Akinci D’Antonoli T, Cuocolo R, Baessler B, Pinto Dos Santos D (2023) Towards reproducible radiomics research: introduction of a database for radiomics studies. Eur Radiol 34:436–443. https://doi.org/10.1007/s00330-023-10095-3
10. 	Wilkinson MD, Dumontier M, Aalbersberg IjJ, et al (2016) The FAIR Guiding Principles for scientific data management and stewardship. Sci Data 3:160018. https://doi.org/10.1038/sdata.2016.18
11. 	Pinto Dos Santos D, Dietzel M, Baessler B (2021) A decade of radiomics research: are images really data or just patterns in the noise? Eur Radiol 31:1–4. https://doi.org/10.1007/s00330-020-07108-w
12. 	Woznicki P, Laqua FC, Al-Haj A, et al (2023) Addressing challenges in radiomics research: systematic review and repository of open-access cancer imaging datasets. Insights Imaging 14:216. https://doi.org/10.1186/s13244-023-01556-w
13. 	European Organization For Nuclear Research, OpenAIRE (2013) Zenodo: Research. Shared.
14. 	Herrick R, Horton W, Olsen T, et al (2016) XNAT Central: Open sourcing imaging research data. NeuroImage 124:1093–1096. https://doi.org/10.1016/j.neuroimage.2015.06.076
15. 	Clark K, Vendt B, Smith K, et al (2013) The Cancer Imaging Archive (TCIA): Maintaining and Operating a Public Information Repository. J Digit Imaging 26:1045–1057. https://doi.org/10.1007/s10278-013-9622-7


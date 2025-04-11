---
title: Item#29
layout: home
parent: 9. Open Science
nav_order: 2
---

Item #29
“Code availability” [1] (licensed under CC BY)
Explanation
“Whether all scripts related to automatic segmentation and/or modeling are shared with the public. These should include clear instructions for their implementation (e.g., accompanying documentation, tutorials).” [1] (licensed under CC BY)
Positive examples from the literature
Example #1: “The used source codes are available at GitHub (https://github.com/tt1107/wangradiology).” [2] (licensed under CC BY)
Example #2: “The implementations can be found at https://github.com/Astarakee/Radiomics_pipeline” [3] (licensed under CC BY)
Example #3: “Sample images, demo codes, and notebook implementations are available at: https://github.com/BoranSekeroglu/OSTEO_MODELS.” [4] (licensed under CC BY-NC)
Example #4: “The complete list of features and the source code is available in GitHub (https://github.com/aydindemircioglu/radPretrained.” [5] (licensed under CC BY)
Hypothetical negative examples
Example #5: The proprietary algorithms used for automated lesion segmentation and the code for the machine learning models are available from the corresponding author upon reasonable request and signing a data/code use agreement.
Example #6: Our novel deep learning architecture for tumor classification was implemented using Python and the PyTorch library. Key hyperparameters and architectural details are described in the Methods section. (No link or statement about code sharing is provided).
Example #7: The analysis scripts can be accessed at the following repository: [Link leads to a 404 Not Found error or an empty repository].
Importance of the item
Code availability is critical in radiomics research due to increasing complexity and reproducibility challenges in medical image analysis [6, 7]. Sharing computational scripts and analysis pipelines enables researchers to validate results, understand methodological nuances, and build upon existing work [8, 9]. By making code publicly accessible, researchers can reduce methodological bias, enhance scientific transparency, and facilitate independent verification of scientific findings. While some studies like the described examples provide comprehensive GitHub repositories with complete code and scripts, many others offer code only upon (reasonable) request, creating barriers to comprehensive scientific review and collaborative advancement in radiomics research.
Specifics about the positive examples
Examples #1 and #2 present the primary source code for implementing traditional radiomics analysis. Feature extraction details are also included. Example #3 offers code for deep learning-based analysis. Although it serves as a foundational study comparing traditional and deep learning methods, Example #4 includes code for both approaches, accompanied by detailed experimental information.
Specifics about the negative examples
In Example #5, the code is not publicly available; access is gated behind contacting the author and signing an agreement, which creates barriers to reproducibility. In Example #6, the item's requirement fails because no information regarding code availability or access location (like a repository link) is provided at all, preventing verification or reuse. In Example #7, the provided link is non-functional (broken or leads to an empty repository), making the code effectively inaccessible despite the stated intention to share.
Recommendations for appropriate scoring
Publications that only offer code "upon reasonable request" to the corresponding author should receive zero (METRICS) points, as this creates arbitrary access barriers and undermines reproducibility principles. Broken links should receive zero points as well.
Item score should be awarded exclusively to studies providing public access to well-documented code repositories (e.g., GitHub) with clear implementation instructions, comprehensive documentation, and thoroughly commented scripts. 
References
{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Wang T, She Y, Yang Y, et al (2022) Radiomics for Survival Risk Stratification of Clinical and Pathologic Stage IA Pure-Solid Non-Small Cell Lung Cancer. Radiology 302:425–434. https://doi.org/10.1148/radiol.2021210109
3. 	Astaraki M, Yang G, Zakko Y, et al (2021) A Comparative Study of Radiomics and Deep-Learning Based Methods for Pulmonary Nodule Malignancy Prediction in Low Dose CT Images. Front Oncol 11:737368. https://doi.org/10.3389/fonc.2021.737368
4. 	Küçükçiloğlu Y, Şekeroğlu B, Adalı T, Şentürk N (2024) Prediction of osteoporosis using MRI and CT scans with unimodal and multimodal deep-learning models. Diagn Interv Radiol 30:9–20. https://doi.org/10.4274/dir.2023.232116
5. 	Demircioğlu A (2022) Predictive performance of radiomic models based on features extracted from pretrained deep networks. Insights Imaging 13:187. https://doi.org/10.1186/s13244-022-01328-y
6. 	Akinci D’Antonoli T, Cuocolo R, Baessler B, Pinto Dos Santos D (2024) Towards reproducible radiomics research: introduction of a database for radiomics studies. Eur Radiol 34:436–443. https://doi.org/10.1007/s00330-023-10095-3
7. 	Kocak B, Chepelev LL, Chu LC, et al (2023) Assessment of RadiomIcS rEsearch (ARISE): a brief guide for authors, reviewers, and readers from the Scientific Editorial Board of European Radiology. Eur Radiol 33:7556–7560. https://doi.org/10.1007/s00330-023-09768-w
8. 	Kocak B, Yardimci AH, Yuzkan S, et al (2023) Transparency in Artificial Intelligence Research: a Systematic Review of Availability Items Related to Open Science in Radiology and Nuclear Medicine. Acad Radiol 30:2254–2266. https://doi.org/10.1016/j.acra.2022.11.030
9. 	Venkatesh K, Santomartino SM, Sulam J, Yi PH (2022) Code and Data Sharing Practices in the Radiology Artificial                     Intelligence Literature: A Meta-Research Study. Radiology: Artificial Intelligence 4:e220081. https://doi.org/10.1148/ryai.220081



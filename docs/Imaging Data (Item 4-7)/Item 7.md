---
title: Item#7
layout: home
parent: 2. Imaging Data
nav_order: 4
---

### Item #7
“The interval between imaging used and reference standard.” [1]  (licensed under CC BY)

### Explanation
“Whether the time interval between the diagnostic imaging exams (used as an input for the radiomics analysis) and the outcome measure/reference standard acquisition is appropriate to validate the presence or absence of target conditions of the radiomics analysis at the moment of the diagnostic imaging exams.” [1]  (licensed under CC BY)

### Positive examples from the literature 
> **Example #1:** “The exclusion criteria were: (a) previous history of radiation therapy, chemotherapy, or biopsy before baseline CT; (b) time interval greater than 2 weeks between the CT examination and surgery” [2] (licensed under CC BY)

> **Example #2:** “Each patient was selected according to the following inclusion criteria: (1) had an accurate history of hypertension (hypertension was defined as systolic pressure ≥ 140 mmHg or diastolic pressure ≥ 90 mmHg); (2) had received their first CT scan within 24 h of disease onset; (3) had completed a CT re-examination within 24 h of disease onset” [3] (licensed under CC BY)

> **Example #3:** “The study included consecutive patients with biopsy-proven PCa enrolled on the local AS programme with a minimum follow-up of 2 years, with their first and last 3T MRI scans performed on the same magnet, and at least one repeat targeted biopsy performed within a year of the last MRI” [4] (licensed under CC BY)

> **Example #4:** “The patients were regularly checked for a LF in intervals of 3 months after finishing RT. LF was determined by individual radiologic review by board-certified radiologists in the specific centers or by histologic results after recurrence surgery. FFLF was calculated as the time difference between the end of SRT and LF. If no LF occurred, patients were right-censored after the last available imaging follow-up. The date of the diagnosis in the MRI was used as time point for LF.” [5] (licensed under CC BY-NC)

### Hypothetical negative examples
> **Example #5:** We investigated the use of radiomics from brain MRI to differentiate between various types of dementia. Patients presenting with cognitive impairment who underwent a brain MRI were included in this retrospective analysis. Radiomic features were extracted from T1-weighted and FLAIR images. The diagnosis of dementia subtype (Alzheimer's disease, vascular dementia, frontotemporal dementia, etc.) was based on the clinical diagnosis made by the treating neurologist at any point during the patient's care.

> **Example #6:** “In this retrospective investigation assessing radiomic features in patients with suspected liver metastases, the primary CT scan was obtained before the confirmatory biopsy.”

> **Example #7:** “This study aimed to assess the ability of radiomic features from baseline CT scans to predict the response to neoadjuvant chemotherapy in patients with locally advanced esophageal cancer. Patients with biopsy-proven esophageal adenocarcinoma who underwent a baseline CT scan and received at least two cycles of neoadjuvant chemotherapy were included. Radiomic features were extracted from the pre-treatment CT scans. Treatment response was assessed using the RECIST 1.1 criteria based on a CT scan performed after completion of all planned chemotherapy cycles.”

### Importance of the item
In radiomics, the time interval between diagnostic imaging exams and outcome measure/reference standard acquisition is crucial for achieving accurate and clinically meaningful results [6]. A shorter interval ensures that imaging features accurately reflect the biological state of the disease or tissue at the time of the reference standard, which is essential for precise outcome prediction [7]. Clinically, a shorter interval aligns imaging findings more closely with the patient’s current condition, providing a more reliable basis for treatment decisions [8]. Additionally, it reduces data noise, as longer intervals allow for disease changes due to treatment or natural progression, potentially distorting imaging features [9]. However, longer intervals may be appropriate when assessing the impact of radiomics on overall survival outcomes [10].

### Specifics about positive examples
Example #1 illustrates an ideal case, as a time interval of less than two weeks between the CT exam and surgery optimally supports assessing the impact of radiomic signatures in diagnosing invasive lung adenocarcinoma. Similarly, minimizing the time between symptom onset and first and second CT scans is crucial for identifying imaging biomarkers that may influence patient prognosis, as the authors did in Example #2 for predicting intracranial hematoma expansion. In the context of active surveillance for clinically insignificant prostate cancer, a minimum follow-up of 2 years adopted in Example #3 represents a reasonable approach to assess the accuracy of MRI delta radiomics models for disease progression prediction. As illustrated in Example #4, imaging follow-up schedules should be clearly defined based on specific guidelines when identifying imaging biomarkers predictive of therapy failure in local disease control. 

### Specifics about the negative examples
In Example #5, the diagnosis of dementia subtype was established at an unspecified later stage, making it unclear whether the radiomic features truly reflected the disease state at the time of imaging. Example #6 lacks a discussion of how much time passed between the primary CT scan and the biopsy. Example #7 does not clarify the interval between baseline imaging and the post-chemotherapy assessment, so there is no way to know if the extracted radiomic features remained representative of the tumor’s condition throughout treatment.	

### Recommendations for appropriate scoring
In general, since no single time interval suits all situations, this should be selected based on the specific clinical scenario and desired outcome. For diagnostic purposes, the interval between imaging and the outcome measure or reference standard acquisition should be as short as possible. Conversely, for prognostic purposes, longer intervals may be necessary, depending on the evidence supporting their clinical relevance. 
An exception may be found in deep learning studies focused on automatic segmentation, where the reference standard is a manual approach, making the concept of interval time irrelevant in such cases. Consequently, the METRICS item related to time interval can be considered met, as it is effectively zero.

### References

{: .fs-2 }


1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Wu G, Woodruff HC, Shen J, et al (2020) Diagnosis of Invasive Lung Adenocarcinoma Based on Chest CT Radiomic Features of Part-Solid Pulmonary Nodules: A Multicenter Study. Radiology 297:451–458. https://doi.org/10.1148/radiol.2020192431
3. 	Yu F, Yang M, He C, et al (2024) CT radiomics combined with clinical and radiological factors predict hematoma expansion in hypertensive intracerebral hemorrhage. Eur Radiol 35:6–19. https://doi.org/10.1007/s00330-024-10921-2
4. 	Sushentsev N, Rundo L, Blyuss O, et al (2022) Comparative performance of MRI-derived PRECISE scores and delta-radiomics models for the prediction of prostate cancer progression in patients on active surveillance. Eur Radiol 32:680–689. https://doi.org/10.1007/s00330-021-08151-x
5. 	Buchner JA, Kofler F, Mayinger M, et al (2024) Radiomics-based prediction of local control in patients with brain metastases following postoperative stereotactic radiotherapy. Neuro-Oncology 26:1638–1650. https://doi.org/10.1093/neuonc/noae098
6. 	Zwanenburg A, Vallières M, Abdalah MA, et al (2020) The Image Biomarker Standardization Initiative: Standardized Quantitative Radiomics for High-Throughput Image-based Phenotyping. Radiology 295:328–338. https://doi.org/10.1148/radiol.2020191145
7. 	Sen A, Troncoso P, Venkatesan A, et al (2021) Correlation of in-vivo imaging with histopathology: A review. European Journal of Radiology 144:109964. https://doi.org/10.1016/j.ejrad.2021.109964
8. 	Russo L, Charles-Davies D, Bottazzi S, et al (2024) Radiomics for clinical decision support in radiation oncology. Clinical Oncology 36:e269–e281. https://doi.org/10.1016/j.clon.2024.03.003
9. 	Xin Y, Li K, Huang M, et al (2023) Biophysics in tumor growth and progression: from single mechano-sensitive molecules to mechanomedicine. Oncogene 42:3457–3490. https://doi.org/10.1038/s41388-023-02844-x
10. 	Le VH, Kha QH, Minh TNT, et al (2023) Development and Validation of CT-Based Radiomics Signature for Overall Survival Prediction in Multi-organ Cancer. J Digit Imaging 36:911–922. https://doi.org/10.1007/s10278-023-00778-0

[Back](https://radiomic.github.io/METRICS-E3/){: .btn .btn-purple  .mr-5  }
[Next](https://radiomic.github.io/METRICS-E3/docs/Study%20Design%20(Item%201-3)/Item%202.html){: .btn .btn-purple   }
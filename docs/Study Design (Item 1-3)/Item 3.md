---
title: Item#3
layout: home
parent: 1. Study Design
nav_order: 3
---

### Item #3
“High-quality reference standard with a clear definition.” [1]  (licensed under CC BY)

### Explanation
“Whether the reference standard or outcome measure is representative of the current clinical practice and robust. Examples of high-quality reference standards are preferably histopathology, well-established clinical and genomic markers, the latest version of the prognostic tools, guideline-based follow-up or consensus-based expert opinions. Examples of poor quality reference standards are those based on qualitative image evaluation, images that are later used for feature extraction, or outdated versions of prognostic tools.” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “Pathology reports were analyzed to assess if EPE was identified on RP specimens at the location of the index lesion, based on the International Society of Urological Pathology consensus conference criteria.” [2] (licensed under CC BY)

> **Example #2:** “Patients with PTB were diagnosed with having a positive smear or tuberculosis culture in at least one respiratory tract sample (sputum or alveolar lavage fluid or lung puncture fluid). […] Adults over 18 years of age with clinical signs suggestive of CAP, acquired outside the hospital or less than 48 hours after admission, meet CAP criteria.” [3] (licensed under CC BY)

> **Example #3:** “Patients with CD in the two centers received standard IFX induction at the weeks 0–2 to 2–6, with a dosage of 5 mg/kg. At week 14, clinical symptoms, endoscopy, laboratory examination, and anti-IFX drug levels were collected from each patient to assess the efficacy of IFX therapy. Additionally, information was collected on whether IFX was used as monotherapy or in combination with an immunomodulator. Patients who did not show satisfactory improvement in a global physician assessment and required treatment changes such as dose escalation, corticosteroid addition, agent switch, or surgery were defined as having PNR. Otherwise, they were classified as primary response to IFX (PR). Besides, patients categorized as PR also needed to conform to the decrease of 50% in SES-CD relative to the baseline as recommended in expert consensus and prior reported clinical trials. Two gastroenterologists (C. Z. and H. Q.) retrospectively evaluated the SES-CD through the report description and endoscopic pictures.” [4] (licensed under CC BY)

> **Example #4:** LTP was defined as any new tumour foci occurring in a 10 mm vicinity of the AZ on follow-up imaging within 24 months after thermal ablation [9]. Lesions were categorized as no LTP if the patient developed (1) no new CRLM; (2) new CRLM > 10 mm distance to the AZ; or (3) new CRLM within 10 mm of the AZ after > 24 months. Follow-up imaging consisted of regular follow-up ceCT, scheduled every 3 months in the first year, and 6 monthly thereafter until 5 years after ablation. In case of doubt, magnetic resonance imaging (MRI) or positron emission tomography (PET)-CT was used as a problem-solver. All liver imaging until the end of follow-up was checked for disease progression.” [5] (licensed under CC BY)

### Hypothetical negative examples
> **Example #5:** Lesions were categorized as malignant or benign based on qualitative radiologist interpretation of imaging features, without histopathological confirmation or longitudinal follow-up.

> **Example #6:** Osteoarthritis severity was categorized based on patient-reported knee pain levels.

> **Example #7:** Lung nodule malignancy was classified based on prior radiology reports from a single institution. Reports were written by different radiologists with varying levels of experience.

### Importance of the item
Reference standard represents a critical source of potential bias in AI [6], and this concept undoubtedly applies to radiomics as well [7]. Thus, researchers should make every effort to adopt the highest quality reference reasonably achievable [8]. Intuitively, this means that the best reference standard will vary depending on the specific clinical task and selected radiomics application. Histopathological results should be preferred and available in those clinical scenarios in which they are routinely used (e.g., characterization of suspicious lesions at prostate MRI). While obtaining histopathological results for all pertinent lesions is not always practical (e.g., low-risk lesions in low-risk patients), a suitable follow-up can represent a solution in these instances. On the other hand, reference standards could be reasonably obtained from experts establishing in consensus the presence of visual imaging features that are diagnostic in selected contexts covered by recognized guidelines (e.g., hepatocellular carcinoma in high-risk patients). There are also conditions for which the reference standard will be represented by clinical and/or laboratory findings (e.g., infectious diseases). However, a valid reference standard should not only be appropriate but also robust and reproducible. Robustness should be ensured by adherence to guidelines, while reproducibility is facilitated by detailed reporting of the methodology employed (e.g., how tissue samples were obtained and processed).

### Specifics about the positive examples
Example #1 illustrates a quite common situation in radiomics applications to oncologic imaging, as only histopathological assessment of prostatectomy specimens could classify the condition reliably, especially since it was performed according to current guidelines. Conversely, in a non-oncological setting, Example #2 depicts the correct use of a combined clinical and laboratory evaluation to classify patients with respiratory diseases. Example #3 depicts a careful assessment of treatment response, in which multiple conditions need to be verified in order to assign a patient to the responders group, reducing the risk of misclassification. Finally, a proper use of imaging features evaluation and follow-up is offered in Example #4, where the follow-up schedule and imaging features criteria for classification were reasonably established as well as clearly reported.

### Specifics about the negative examples
These examples represent poor-quality reference standards due to their lack of objective validation, potential bias, and inconsistency. In Example #5, lesion classification relies solely on radiologist interpretation without histopathological confirmation or follow-up, making the diagnosis subjective and prone to misclassification. Example #6 categorizes osteoarthritis severity based on patient-reported pain levels, which are inherently subjective and do not directly correlate with structural joint damage; a more reliable approach would involve imaging or clinical grading systems. Example #7 uses prior radiology reports from a single institution, where different radiologists with varying levels of experience may have applied inconsistent classification criteria, leading to variability and potential bias in the reference standard. Without robust validation, these approaches introduce significant risks of error and compromise the reliability of radiomics or AI models trained on such data.

### Recommendations for appropriate scoring
As elucidated above, there is no reference standard that could fit all scenarios, and its validity should thus be critically evaluated per case. However, there are some characteristics that define reliable and robust reference standards. Firstly, they should be clinically validated and widely accepted within the field. A precise definition relevant to the research question should be provided. Then, it should explicitly describe how it was implemented and the choice justified for its relevance to the outcomes analyzed. 

As for any research study, consistently applying the reference standard across all cases reduces the risk of bias. If there are concerns, identifying and acknowledging potential bias increases transparency and improves results interpretation. When reference standards are obtained in clinical practice, independent validation within the study might bring added value. Finally, when the reference standard is not as robust as desired, the inclusion of uncertainty estimation in the model’s training/evaluation could be considered.

This item may be considered somewhat subjective due to the vagueness of the term “high-quality.” However, assessing this criterion requires a certain level of domain knowledge relevant to the study of interest. A study should receive a score for item #3 if it employs a high-quality reference standard that is clinically relevant, clearly defined, consistently applied, and, where applicable, independently validated. A study should receive no score if it relies on a weak, poorly defined, inconsistently applied, or subjective reference standard without proper justification or efforts to address potential bias and uncertainty.

### References
1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Cuocolo R, Stanzione A, Faletti R, et al (2021) MRI index lesion radiomics and machine learning for detection of extraprostatic extension of disease: a multicenter study. Eur Radiol 31:7575–7583. https://doi.org/10.1007/s00330-021-07856-3
3. 	Li P, Wang J, Tang M, et al (2024) A CT-based radiomics predictive nomogram to identify pulmonary tuberculosis from community-acquired pneumonia: a multicenter cohort study. Front Cell Infect Microbiol 14:1388991. https://doi.org/10.3389/fcimb.2024.1388991
4. 	Wang Y, Luo Z, Zhou Z, et al (2024) CT-based radiomics signature of visceral adipose tissue and bowel lesions for identifying patients with Crohn’s disease resistant to infliximab. Insights Imaging 15:28. https://doi.org/10.1186/s13244-023-01581-9
5. 	Van Der Reijd DJ, Guerendel C, Staal FCR, et al (2023) Independent validation of CT radiomics models in colorectal liver metastases: predicting local tumour progression after ablation. Eur Radiol 34:3635–3643. https://doi.org/10.1007/s00330-023-10417-5
6. 	Koçak B, Ponsiglione A, Stanzione A, et al (2024) Bias in artificial intelligence for medical imaging: fundamentals, detection, avoidance, mitigation, challenges, ethics, and prospects. dir. https://doi.org/10.4274/dir.2024.242854
7. 	Papanikolaou N, Matos C, Koh DM (2020) How to develop a meaningful radiomic signature for clinical use in oncologic patients. Cancer Imaging 20:33. https://doi.org/10.1186/s40644-020-00311-4
8. 	Koçak B, Cuocolo R, Santos DPD, et al (2023) Must-have Qualities of Clinical Research on Artificial Intelligence and Machine Learning. Balkan Med J 40:3–12. https://doi.org/10.4274/balkanmedj.galenos.2022.2022-11-51

[Previous: Item #2](https://radiomic.github.io/METRICS-E3/docs/Study%20Design%20(Item%201-3)/Item%202.html){: .btn .btn-purple  .mr-5  }
[Next: Item #4](https://radiomic.github.io/METRICS-E3/docs/Imaging%20Data%20(Item%204-7)/Item%204.html){: .btn .btn-purple   }


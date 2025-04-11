---
title: Item#4
layout: home
parent: 2. Imaging Data
nav_order: 1
---
## Item #4
“Multi-center.” [1]  (licensed under CC BY)

### Explanation
“Whether more than one institution is involved as a diagnostic imaging data source for radiomics analysis.” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “Data collection was approved by the institutional review board of each of the main contributing medical centers approached for retrospective collection University Medical Center Groningen (UMCG, Groningen, The Netherlands) and Martini Hospital Groningen (Groningen, The Netherlands). Informed consent was waived due to the retrospective nature of the study. Because of clinical suspicion of PCa, a group of 930 patients, which consisted almost exclusively of white European males, was investigated between 2014 and 2020 using a combination of MRI (9 hospitals, 2 vendors, 8 types; Additional file 1) and systematic or targeted biopsy techniques.” [2] (licensed under CC BY)

> **Example #2:** “A cohort of 197 patients with locally advanced cervical cancer from 3 centers (Brest, n = 119 and Nantes, n = 50, in France, and Montreal, n = 28, in Canada) was exploited.” [3] (licensed under CC BY)

> **Example #3:** “A total of 261 NPC patients who received RT at Hong Kong Queen Elizabeth Hospital (QEH) between 2012 and 2015 and 160 NPC patients who received RT at Hong Kong Queen Mary Hospital (QMH) between 2012 and 2020 were retrospectively screened for study eligibility.” [4] (licensed under CC BY)

### Hypothetical negative examples
> **Example #4:** This retrospective study included 350 patients diagnosed with hepatocellular carcinoma at a single tertiary medical center. External validation was performed by randomly splitting the data in a ratio of 7:3.

> **Example #5:** A total of 420 patients with lung cancer were retrospectively collected from two affiliated hospitals within the same local healthcare network. Both hospitals used the similar imaging protocols and scanners for data acquisition.

### Importance of the item
Radiomic models are often sensitive to variations in imaging protocols and scanner types, which can limit their performance when applied to data from a single institution [5–7]. For this reason, multicenter analysis, by including different populations, scanners and acquisition protocols, is crucial for ensuring the generalizability and robustness of predictive models across diverse patient populations and imaging conditions [7, 8]. Incorporating data from multiple centers helps in reducing biases and improving the real-world applicability of radiomics analysis fields [8, 9].

### Specifics about the positive examples
Example #1 involved data from two major hospitals in the Netherlands. Example #2 leveraged a cohort from three centers in different countries, France and Canada, without specific details of the source hospitals. Finally, Example #3 combined data from two hospitals in Hong Kong.

### Specifics about the negative examples
Example #4 is a negative example because it is entirely based on data from a single institution, meaning it does not qualify as a multi-center study. The mention of “external validation” is misleading, as the validation was performed through an internal hold-out split (7:3), rather than using data from an independent institution. Example #5 is also a negative example because, although it includes data from two hospitals, they belong to the same healthcare network and use similar imaging protocols and scanners. This results in a homogeneous dataset that lacks the variability expected in a true multi-center study, where differences in patient populations, imaging equipment, and acquisition protocols help improve the robustness and generalizability of radiomic models.

### Recommendations for appropriate scoring
A key concern is the classification of so-called multicenter studies that include only affiliated hospitals or parts of a larger healthcare system, particularly when these institutions share similar distributions in patient characteristics, imaging scanners, and protocols. Such cases should be carefully evaluated and, if necessary, classified as single-center studies under their main hospital to ensure methodological accuracy.
Another concern is the use of the term “external validation” or “external testing” in the studies, suggesting a multi-center design. Nevertheless, these terms may be misused to describe standard hold-out validation in single-center studies. METRICS evaluators should critically assess whether multiple centers are genuinely involved rather than relying solely on the terminology used in the manuscript.

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Bleker J, Yakar D, Van Noort B, et al (2021) Single-center versus multi-center biparametric MRI radiomics approach for clinically significant peripheral zone prostate cancer. Insights Imaging 12:150. https://doi.org/10.1186/s13244-021-01099-y
3. 	Da-ano R, Masson I, Lucia F, et al (2020) Performance comparison of modified ComBat for harmonization of radiomic features for multicenter studies. Sci Rep 10:10248. https://doi.org/10.1038/s41598-020-66110-w
4. 	Lam S-K, Zhang J, Zhang Y-P, et al (2022) A Multi-Center Study of CT-Based Neck Nodal Radiomics for Predicting an Adaptive Radiotherapy Trigger of Ill-Fitted Thermoplastic Masks in Patients with Nasopharyngeal Carcinoma. Life 12:241. https://doi.org/10.3390/life12020241
5. 	Kocak B, Pinto dos Santos D, Dietzel M (2025) The widening gap between radiomics research and clinical translation: rethinking current practices and shared responsibilities. European Journal of Radiology Artificial Intelligence 1:100004. https://doi.org/10.1016/j.ejrai.2025.100004
6. 	Kocak B, Akinci D’Antonoli T, Ates Kus E, et al (2024) Self-reported checklists and quality scoring tools in radiomics: a meta-research. Eur Radiol 34:5028–5040. https://doi.org/10.1007/s00330-023-10487-5
7. 	van Timmeren JE, Cester D, Tanadini-Lang S, et al (2020) Radiomics in medical imaging—“how-to” guide and critical reflection. Insights into Imaging 11:91. https://doi.org/10.1186/s13244-020-00887-2
8. 	Koçak B (2022) Key concepts, common pitfalls, and best practices in artificial intelligence and machine learning: focus on radiomics. Diagn Interv Radiol 28:450–462. https://doi.org/10.5152/dir.2022.211297
9. 	Lambin P, Rios-Velazquez E, Leijenaar R, et al (2012) Radiomics: Extracting more information from medical images using advanced feature analysis. European Journal of Cancer 48:441–446. https://doi.org/10.1016/j.ejca.2011.11.036


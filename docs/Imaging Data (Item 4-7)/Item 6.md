---
title: Item#6
layout: home
parent: 2. Imaging Data
nav_order: 3
---

## Item #6
“Imaging protocol with acquisition parameters” [1] (licensed under CC BY)
### Explanation
“Whether the image acquisition protocol is clearly reported to ensure the replicability of the method.” [1]  (licensed under CC BY)
### Positive examples from the literature
> **Example #1:** “Apart from the echo time, two T2-weighted sequences were used (TE75, TE300) with a field-of-view of 400 × 400 × 233 (AP × RL × FH) mm, a reconstructed in-plane voxel of 1 × 1 (AP × RL) mm, slice thickness of 5 mm FH, echo times of 75 and 300 ms respectively and a repetition time of 2725 ms, without fat suppression. Five routinely available sequences were collected from the diffusion-weighted scan (b0, b10, b200, b800, and ADC) with a field-of-view of 450 × 400 × 251 (AP × RL × FH) mm, reconstructed in-plane voxel size of 1.75 × 1.75 (AP × RL) mm, echo time of 86 ms, repetition time of 1447 ms, and a SPAIR fat suppression pulse was used—leading to a maximum of seven sequences available per liver resection.” [2] (licensed under CC BY)

> **Example #2** See Table 1. 
Table 1. “Scanning parameters” [3] (licensed under CC BY)

 

> **Example #3:** See Table 2.
Table 2. “Imaging protocol of the 32 CT scans.” [4] (licensed under CC BY)
 
> **Example #4:** See Table 3.
Table 3. “CT scan characteristics based on data source cites.” [5] (licensed under CC BY)
 

### Hypothetical negative examples
Example #5: Patients underwent pre-operative MRI examinations using a clinical MRI scanner. Both T1-weighted and T2-weighted images were acquired as part of the standard protocol. For the T1-weighted images, we used a relatively short repetition time to maximize T1 contrast. The echo time was kept short to minimize T2 effects. Slice thickness was approximately 5mm. For the T2-weighted images, a longer repetition time and echo time were selected, appropriate for visualizing T2 contrast. Diffusion-weighted imaging was also performed, using multiple b-values to assess apparent diffusion coefficient (ADC). A contrast agent was administered intravenously to a subset of the patients, depending on the referring physician's request. Images were reconstructed using the scanner's standard reconstruction algorithm.
Example #6: All patients underwent CT scanning prior to treatment. Scans were acquired using helical acquisition mode on multi-detector CT scanners available at the participating institutions. A standard abdominal protocol was employed, with adjustments made for patient size and clinical indication. Intravenous contrast material was administered in most cases, unless contraindicated. Slice thickness was generally around 5mm, although thinner slices were sometimes acquired for specific regions of interest. Tube voltage was typically 120 kVp, and tube current was adjusted automatically by the scanner's dose modulation system. Images were reconstructed using a standard soft-tissue kernel.
### Importance of the item 
Generalizability of radiomics features is susceptible to differences in acquisition protocols [6]. It is important to report what specific acquisition protocols are used on what type of scanners, because researchers aiming to reproduce or validate results in papers require this essential information to put their results in context. 
Specifics about the positive examples
Example #1 illustrates well how MR parameters could be reported fully in a concise manner. Specifically in MR imaging, where sequences are often optimized per center, complete reporting of all parameters is strongly encouraged. Example #2 visualized the different CT scanners used in each of the different datasets, indicating where CT scanners were in or out of distribution compared to the training cohort. This overview yields insights into the generalizability of the method and on what cohorts, what performances can be expected. In Example #3, a concise table with the required CT parameters is displayed, with an essential split on the scanner type. Even better, Example #4 splits the scanner type per source in their multicenter study, where this table yields an excellent overview of all the recommended CT parameters to report.
### Specifics about the negative examples
In Example #5, the MRI acquisition parameters are vaguely described, with terms like relatively short repetition time and approximately 5mm slice thickness, instead of providing precise numerical values. Additionally, key parameters such as field strength, in-plane resolution, echo train length, and diffusion b-values are missing. In Example #6, the CT protocol is similarly imprecise, with general terms like standard abdominal protocol and tube current adjusted automatically, without specifying exact values, scanner models, or algorithm used. 
### Recommendations for appropriate scoring
Authors should report all the scanner types and acquisition protocol of all scans included in the dataset. It should be clear what acquisition protocols were used in the training, test, and external validation datasets. For CT, kVp, mA, in-plane resolution, slice thickness, reconstruction kernel (soft, lung, bone), and use of contrast should be reported. For MR, the type of sequence, echo time, in-plane resolution, slice thickness, field of view, repetition time, use of contrast, use of fat suppression, magnetic field strength, diffusion parameters, flip angle, and reconstruction algorithm. When the main body does not allow for it, extensive tables in the supplemental materials are advised.
### References
1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Bodalal Z, Bogveradze N, Ter Beek LC, et al (2023) Radiomic signatures from T2W and DWI MRI are predictive of tumour hypoxia in colorectal liver metastases. Insights Imaging 14:133. https://doi.org/10.1186/s13244-023-01474-x
3. 	van der Reijd DJ, Guerendel C, Staal FCR, et al (2024) Independent validation of CT radiomics models in colorectal liver metastases: predicting local tumour progression after ablation. Eur Radiol 34:3635–3643. https://doi.org/10.1007/s00330-023-10417-5
4. 	Lu L, Ehmke RC, Schwartz LH, Zhao B (2016) Assessing Agreement between Radiomic Features Computed for Multiple CT Imaging Settings. PLOS ONE 11:e0166550. https://doi.org/10.1371/journal.pone.0166550
5. 	Lu L, Ahmed FS, Akin O, et al (2021) Uncontrolled Confounders May Lead to False or Overvalued Radiomics Signature: A Proof of Concept Using Survival Analysis in a Multicenter Cohort of Kidney Cancer. Front Oncol 11:638185. https://doi.org/10.3389/fonc.2021.638185
6. 	Berenguer R, Pastor-Juan MDR, Canales-Vázquez J, et al (2018) Radiomics of CT Features May Be Nonreproducible and Redundant: Influence of CT Acquisition Parameters. Radiology 288:407–415. https://doi.org/10.1148/radiol.2018172361

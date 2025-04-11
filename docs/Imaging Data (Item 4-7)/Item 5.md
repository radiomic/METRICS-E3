---
title: Item#5
layout: home
parent: 2. Imaging Data
nav_order: 2
---

### Item #5
“Clinical translatability of the imaging data source for radiomics analysis” [1]  (licensed under CC BY)

### Explanation
“Whether the source of the radiomics data is an imaging technique that reflects established standardization approaches, such as acquisition protocol guidelines (e.g., PI-RADS specifications).” [1]  (licensed under CC BY)

### Positive examples from the literature
> **Example #1:** “The MRI protocol was optimized following international recommendations and current practice in breast MRI. Images were acquired in axial plane and the patient in a prone position using either 1.5 T or 3.0 T scanners (Magnetom Avanto/Aera; Verio/Skyra) and dedicated breast array coils (all hardware: Siemens Healthineers, Erlangen, Germany). Protocols included dynamic contrast-enhanced T1-weighted scans, a T2-weighted fat-saturated scan and diffusion-weighted imaging. Protocol parameters are provided in Table 2. The contrast media (0.1 mmol/kg body weight gadobutrol, Bayer Schering Pharma, Berlin, Germany) was injected into an antecubital vein after the first dynamic acquisition with a flow of 2.0 mL/sec, followed by a 20 mL saline flush. After a 30-second delay, the remaining five dynamic acquisitions were scanned under identical conditions.” [2] (licensed under CC BY)

> **Example #2:** “All patients underwent contrast-enhanced MRI with a dedicated liver protocol, in accordance with LI-RADS v2018 technical recommendations which include the following sequences: axial T2-weighted turbo or fast spin-echo (with and without fat saturation) sequences, axial dual gradient-recalled echo T1-weighted sequence (in-phase and opposed-phase), and axial diffusion weighted imaging acquired with b values of 0, 150 and 800 s/mm2. Axial T1-weighted three-dimensional gradient-recalled echo sequences with fat suppression (Liver Acquisition with Volume Acceleration, LAVA, General Electric; or T1-weighted high-resolution isotropic volume examination, THRIVE, Philips Healthcare) were obtained before and after contrast agent administration. Detailed parameters of T1-weighted three-dimensional gradient-recalled echo sequences are reported in Supplementary Table S1.” [3] (licensed under CC BY)

### Hypothetical negative examples
> **Example #3:** MRI data were acquired using multiple scanners from different vendors, including Siemens Magnetom Skyra, Philips Ingenia, and GE Signa Premier, with field strengths of 1.5T and 3.0T. T1-weighted imaging was performed with repetition times (TR) ranging from 400 ms to 800 ms and echo times (TE) between 8 ms and 20 ms. T2-weighted sequences were obtained using fast spin-echo (FSE) or turbo spin-echo (TSE) techniques, with echo train lengths (ETL) varying from 12 to 25 and slice thicknesses between 3 mm and 5 mm. Diffusion-weighted imaging (DWI) was acquired with different b-values across sites, including combinations of 0, 500, and 1000 s/mm².

> **Example #4:** MRI data were collected as part of a multi-center clinical trial investigating a new contrast agent for liver imaging. Each participating center used its standard clinical protocol for liver MRI, with the only modification being the administration of the investigational contrast agent. Detailed protocol information for each center is provided in the supplementary materials.

> **Example #5:** MRI scans were acquired using a 3T scanner with a dedicated cardiac coil. A standard cine imaging protocol was used to assess left ventricular function. Image acquisition was triggered by the patient's electrocardiogram (ECG). The imaging protocol was developed locally by the radiology department based on best practices for cardiac MRI.

### Importance of the item
The clinical translatability of imaging data ensures that analysis results can be reliably applied in real-world clinical scenarios. Even though homogenization processes can be applied to standardize the image signal, radiomic features are highly susceptible to variations in imaging acquisition, reconstruction, and protocol inconsistencies. As differences may bring unexpected influences on the radiomic model [4], adherence to standardized imaging guidelines, such as PI-RADS or BI-RADS, is crucial to minimize the risk of generating non-reproducible or non-generalizable results across institutions and patient populations [5, 6]. 
### Specifics about the positive examples
In the positive examples, specific mentioning of international protocols are present in Example #1 and Example #2, with detailed tables including the protocol details. 
### Specifics about the negative examples
Example #3 involves multiple scanners with different field strengths and varied sequence parameters, without referring to a guideline or mention of a protocol adherence. Example #4 uses site-specific MRI protocols in a multi-center study with experimental use of a contrast agent, introducing differences in acquisition settings that hinder comparability. Example #5 relies on a locally developed cardiac MRI protocol without adherence to standardized guidelines.
### Recommendations for appropriate scoring
When assessing the clinical translatability of an imaging data source consistently, scoring should prioritize strict adherence to standardized imaging protocols. Studies that explicitly document the use of established guidelines (e.g., acquisition standards like PI-RADS or Lung-RADS), recommendations, or common standards—by citing relevant papers—should receive the score for this METRICS item.

In contrast, studies that do not mention protocol adherence and lack references to relevant papers should not earn the METRICS score.
### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Ellmann S, Wenkel E, Dietzel M, et al (2020) Implementation of machine learning into clinical breast MRI: Potential for objective and accurate decision-making in suspicious breast masses. PLOS ONE 15:e0228446. https://doi.org/10.1371/journal.pone.0228446
3. 	Cannella R, Cammà C, Matteini F, et al (2022) Radiomics Analysis on Gadoxetate Disodium-Enhanced MRI Predicts Response to Transarterial Embolization in Patients with HCC. Diagnostics 12:1308. https://doi.org/10.3390/diagnostics12061308
4. 	He L, Huang Y, Ma Z, et al (2016) Effects of contrast-enhancement, reconstruction slice thickness and convolution kernel on the diagnostic performance of radiomics signature in solitary pulmonary nodule. Sci Rep 6:34921. https://doi.org/10.1038/srep34921
5. 	Mann RM, Kuhl CK, Kinkel K, Boetes C (2008) Breast MRI: guidelines from the European Society of Breast Imaging. Eur Radiol 18:1307–1318. https://doi.org/10.1007/s00330-008-0863-7
6. 	Weinreb JC, Barentsz JO, Choyke PL, et al (2016) PI-RADS Prostate Imaging – Reporting and Data System: 2015, Version 2. European Urology 69:16–40. https://doi.org/10.1016/j.eururo.2015.08.052

[Back](https://radiomic.github.io/METRICS-E3/docs/Imaging%20Data%20(Item%204-7)/Item%204.html){: .btn .btn-purple  .mr-5  }
[Next](https://radiomic.github.io/METRICS-E3/docs/Imaging%20Data%20(Item%204-7)/Item%206.html){: .btn .btn-purple   }

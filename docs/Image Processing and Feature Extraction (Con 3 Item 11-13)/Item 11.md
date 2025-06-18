---
title: Item#11
layout: home
parent: 4. Image Processing and Feature Extraction
nav_order: 2
---

### Item #11
“Appropriate use of image preprocessing techniques with transparent description.” [1]  (licensed under CC BY)

### Explanation
“Whether preprocessing of the images is appropriately performed considering the imaging modality (e.g., gray level normalization for MRI, image registration in case of multiple contrasts or modalities) and feature extraction techniques (i.e., 2D or 3D) that are used. For instance, in the case of large slice thickness (e.g., ≥5 mm), extreme upsampling (e.g., 1 x 1 x 1 mm3) of the volume might be inappropriate. In such a case, 2D feature extraction could be preferable, ensuring in-plane isotropy of the pixels. On the other hand, achieving isotropic voxel values should be targeted in 3D feature extraction, to allow for texture feature rotational invariance. Also, whether gray level discretization parameters (bin width, along with resulting gray level range, or bin count) are described in full detail. Description of the different image types used (e.g., original, filtered) should also be included (e.g., high and low pass filter combinations for wavelet decomposition, sigma values for Laplacian of Gaussian edge enhancement filtering). If the image window is fixed, it should be clarified.” [1]  (licensed under CC BY)

### Positive examples from the literature 
> **Example #1:** “The radiomic profiles were obtained from the semi-automatic delineation volumes of interest (VOIs) following normalization, discretion, and image resampling. To minimize the impact of varying slice thicknesses and voxel sizes on the radiomics profile, decrease dependence of the radiomic profiles on voxel size, and ensure rotational invariance of textural profiles, while retaining the original intensity scale and meaning of voxel values, two distinct discretization strategies were employed for the two quantitative functional imaging modalities (18F-FDG -PET and low dose CT) with fixed bin width (FBW) sizes (bin sizes for PET = 0.25; CT = 25) which may be more suitable in certain circumstances than a fixed bin number for comparative analysis by various modalities. Based on the Image Biomarker Standardization Initiative (IBSI) criteria of image normalization and contrast prioritization inside VOIs, we employed tri-linear interpolation to produce isotropic 3 × 3 × 3 and 2 × 2 × 2 mm voxels in PET and CT scans respectively.” [2] (licensed under CC BY)

> **Example #2:** “Before the feature calculation, the images of each patient were standardized separately to improve the texture recognition rate. Firstly, the T2WI, DWI and ADC images of each patient were resampled to a voxel size of 1 × 1 × 1 cm3 to standardize the voxel spacing. Then the voxel intensity discretization was accomplished by setting the bin width to 25 to reduce imaging noise and standardize the intensity. Finally, through Z-score Normalization for different sequence of each case, which can reduce the influence of the inconsistency of image parameters on the variation of radiomics features, the voxel intensity was transformed into a distribution with 0 as the mean and 1 as the standard deviation. […] The original images were transformed by Wavelet Transform, and 2078 wavelet features are extracted in three spatial directions.” [3] (licensed under CC BY)

> **Example #3:** “The preprocessing of prostate MRI images included data de-identification, registration, data harmonization, and data augmentation (Supplementary Section 4) referring to our previous study. ” […] “All multiparameter MRI images were first converted from Digital Imaging and Communications in Medicine (DICOM) to Neuroimaging Informatics Technology Initiative (NIFTI) format to remove patients' private information. After preprocessing, for each patient, a 3D ROI, including the index lesion, was produced with a resolution of 112×112×16, which met the dimension of the input of the DL model. For each patient, the DWI images and ADC maps derived from DWI with different gradient field parameters were spatially aligned to the T2WI images by a rigid 3D registration method using the SimpleElastix toolbox (http://simpleelastix.github.io/).” […] “Additionally, even in the same center, the size of index lesions also presented great inter-patient variation. The aim of data harmonization is to resample the cuboid 3D regions of interest (ROI) containing the entire index lesion into the common spatial resolution for all patients and thereby meet the dimension of the input of the deep learning model. The data harmonization included three steps: (1) all MRI images were resampled to a common voxel size of 0.46×0.46×3, which was the median value of voxel spacing in the training cohort; (2) for each index lesion, in the slice where the section of the lesion was the largest extent size, a 2D square ROI was produced to comprise the lesion with an additional 5-voxel margin. Then, this 2D ROI was reproduced in the slices containing the lesion with an additional 5-slice margin extending to the top and bottom. Finally, these 2D ROI consisted of a 3D ROI. (3) For all patients, the 3D ROIs were resampled into a common resolution of 112×112×16. (3) For each 3D ROI, the intensity of each voxel was converted to z-score, namely 𝑧‑𝑠𝑐𝑜𝑟𝑒 = 𝑥𝑖−𝑥/σ , where 𝑥𝑖  is the original intensity value of the ith voxel, and 𝑥 and σ are the mean and standard deviation across all voxels of corresponding 3D ROI, respectively.” [4] (licensed under CC BY)

> **Example #4:** “MR images were preprocessed with N4 Bias Field Correction algorithm to correct low frequency intensity. Then, the intensities were normalised were normalised using the Z-score such as Inew = (I−μ)/σ where μ and σ are the mean and standard deviation of the intensities. Regarding the low number of samples and the complexity of images acquired on different body region, we choose to focus on a classification model only based on the tumour. MRI slices were cropped around the tumours with respect to the masks and resized to a unique matrix size (224 × 224 pixels).” [5] (licensed under CC BY)

### Hypothetical negative examples
> **Example #5:** Images were preprocessed before radiomic feature extraction. We normalized the intensities and resampled the images to a uniform size. Features were then calculated from the processed volumes.

> **Example #6:** Images were preprocessed based on the default configuration of the software before radiomic feature extraction. We normalized the intensities and resampled the images to a uniform size. We also used transformed images other than the original ones to extract features.

> **Example #7:** Images were resized to fit the input of our deep learning model. We also applied data augmentation to increase the size of our training dataset. The input images went through a standard normalization pipeline.

### Importance of the item
Preprocessing is a critical step in radiomics and deep learning [6, 7]. Poorly preprocessed data can lead to biased feature extraction and unreliable predictions. Therefore, rigorous preprocessing pipelines are essential to improve model accuracy, facilitate reproducibility, and ensure the clinical applicability of radiomics and AI-based medical imaging models [8]. In traditional radiomics, preprocessing techniques such as intensity normalization, resampling, and discretization help standardize imaging data, reducing variability caused by acquisition settings and scanner differences. Furthermore, the application of preprocessing filters can improve the expected performance from traditional radiomics [9]. In deep learning, preprocessing includes resizing, fixed grey-level windowing, padding, data augmentation, and normalization, which enhance model generalizability and performance. Each imaging modality may also require tailored preprocessing techniques to address specific challenges, such as MRI bias field correction. 

### Specifics about the positive examples
Examples #1 and #2 effectively detail the preprocessing steps for traditional radiomics analysis, emphasizing normalization, resampling, and discretization. Similarly, Examples #3 and #4 outline key preprocessing steps for deep learning-based analysis. Both examples include resampling and normalization, along with resizing. Additionally, Example #4 incorporates bias field correction for MRI data.

### Specifics about the negative examples
Example #5 lacks essential preprocessing details. It mentions normalization and resampling but omits the resampling method, target voxel size, and normalization technique. It also fails to specify intensity discretization, making the preprocessing pipeline non-reproducible.

Example #6 is vague and lacks reproducibility. It refers to default software settings without naming the software, its version, or detailing preprocessing steps. It also mentions transformed images without specifying the type or application method, preventing replication.

Example #7 focuses only on resizing and data augmentation but lacks key preprocessing details for deep learning. It does not specify the original and final image dimensions, interpolation or padding methods, or the type of normalization applied. 

### Recommendations for appropriate scoring
A study should be scored as “Yes” if it includes at least the following details (applied or not applied): for traditional radiomics analysis, resampling size and discretization parameters; for deep learning analysis, resampling, normalization, and resizing as a minimum requirement. If any of these key preprocessing details are missing or insufficiently described, the study should be scored as “No”. 

It is important to note that specific preprocessing steps are relevant to particular imaging modalities, and these should be considered when evaluating this item. 

### References

{: .fs-2 }

1. 	Kocak B, Akinci D’Antonoli T, Mercaldo N, et al (2024) METhodological RadiomICs Score (METRICS): a quality scoring tool for radiomics research endorsed by EuSoMII. Insights Imaging 15:8. https://doi.org/10.1186/s13244-023-01572-w
2. 	Zhong H, Huang D, Wu J, et al (2023) 18F‑FDG PET/CT based radiomics features improve prediction of prognosis: multiple machine learning algorithms and multimodality applications for multiple myeloma. BMC Med Imaging 23:87. https://doi.org/10.1186/s12880-023-01033-2
3. 	Jin P, Shen J, Yang L, et al (2023) Machine learning-based radiomics model to predict benign and malignant PI-RADS v2.1 category 3 lesions: a retrospective multi-center study. BMC Med Imaging 23:47. https://doi.org/10.1186/s12880-023-01002-9
4. 	Bao J, Zhao L, Qiao X, et al (2025) 3D-AttenNet model can predict clinically significant prostate cancer in PI-RADS category 3 patients: a retrospective multicenter study. Insights Imaging 16:25. https://doi.org/10.1186/s13244-024-01896-1
5. 	Fradet G, Ayde R, Bottois H, et al (2022) Prediction of lipomatous soft tissue malignancy on MRI: comparison between machine learning applied to radiomics and deep learning. Eur Radiol Exp 6:41. https://doi.org/10.1186/s41747-022-00295-9
6. 	van Timmeren JE, Cester D, Tanadini-Lang S, et al (2020) Radiomics in medical imaging—“how-to” guide and critical reflection. Insights into Imaging 11:91. https://doi.org/10.1186/s13244-020-00887-2
7. 	Koçak B (2022) Key concepts, common pitfalls, and best practices in artificial intelligence and machine learning: focus on radiomics. Diagn Interv Radiol 28:450–462. https://doi.org/10.5152/dir.2022.211297
8. 	Trojani V, Bassi MC, Verzellesi L, Bertolini M (2024) Impact of Preprocessing Parameters in Medical Imaging-Based Radiomic Studies: A Systematic Review. Cancers 16:2668. https://doi.org/10.3390/cancers16152668
9. 	Demircioğlu A (2022) The effect of preprocessing filters on predictive performance in radiomics. European Radiology Experimental 6:40. https://doi.org/10.1186/s41747-022-00294-w

[Previous: Condition #11](https://radiomic.github.io/METRICS-E3/docs/Image%20Processing%20and%20Feature%20Extraction%20(Con%203%20Item%2011-13)/Condition%203.html){: .btn .btn-purple  .mr-5  }
[Next: Item #12](https://radiomic.github.io/METRICS-E3/docs/Image%20Processing%20and%20Feature%20Extraction%20(Con%203%20Item%2011-13)/Item%2012.html){: .btn .btn-purple   }
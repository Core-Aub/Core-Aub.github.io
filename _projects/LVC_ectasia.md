---
layout: page
title: Raw versus Engineered Tomographic Representations for Post–Laser Vision Correction Ectasia Diagnosis
description: A postoperative, single-exam classification framework for detecting post-laser vision correction ectasia using high-dimensional raw corneal tomography maps and interpretable deep learning.
img: assets/img/post_lvc.jpeg
importance: 1
category: Finished
---

{% include figure.html path="assets/img/post_lvc.jpeg" title="Post-LVC Ectasia Detection from Raw Corneal Tomography" class="img-fluid rounded z-depth-1" %}

**Abstract**

Motivation: Post–laser vision correction (Post-LVC) ectasia is a severe complication that can occur when mild or subclinical ectatic disease (e.g., keratoconus) goes undetected during preoperative screening. Once surgery is performed, the biomechanically weakened cornea may progressively deform, leading to visual deterioration. Current postoperative detection strategies rely primarily on biomechanical measurements, longitudinal follow-up, and expert interpretation. To date, there is no automated, tomography-based, single-exam classification framework designed specifically for postoperative ectasia detection.

Results: We propose a data-driven approach for postoperative Post-LVC ectasia classification using raw corneal tomography maps acquired from the MS39 device. Each examination consists of high-dimensional measurements across radii, angular positions, and multiple map types, resulting in an input tensor of size (25, 256, 16). Given limited sample sizes, directly learning from this representation is impractical. To address this, we apply bicubic interpolation along the angular dimension to compress the data into a lower-dimensional representation of size (25, 30, 16), which is then flattened into a 1D feature vector for TabNet. We benchmark performance against established preoperative risk assessment indices. The proposed approach achieves an F1-score of 96%, outperforming models based on engineered preoperative features, which achieve an F1-score of 93.1%.

Interpretability and Error Analysis: To assess clinical validity and model behavior, we analyze TabNet attention maps corresponding to correctly and incorrectly classified cases. These attention maps reveal anatomically meaningful regions of focus that align with known ectatic deformation patterns, providing insight into the decision-making process of the network. Error analysis further highlights scenarios where subtle postoperative changes challenge both automated and expert assessment, underscoring the difficulty of the task.

{% include figure.html path="assets/img/post_lvc_attention.jpeg" title="TabNet Attention Maps" class="img-fluid rounded z-depth-1" %}

Conclusion: This work introduces the first automated, tomography-only, single-exam framework for Post-LVC ectasia detection. By leveraging raw corneal maps, principled dimensionality reduction, and interpretable deep learning, we demonstrate that postoperative ectasia can be detected with high accuracy and clinically meaningful explanations.

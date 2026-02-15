---
layout: page
title: Learning Corneal Epithelial Remodeling from Stromal Geometry Using Deep Neural Networks
description: A deep learning framework for predicting corneal epithelial elevation directly from stromal geometry, modeling epithelial remodeling as a data-driven image-to-image translation problem with clinical relevance for surgical planning.
img: assets/img/Stroma.jpeg
importance: 1
category: Ongoing
---

{% include figure.html path="assets/img/Stroma.jpeg" title="Deep Learning-Based Corneal Epithelial Remodeling Prediction" class="img-fluid rounded z-depth-1" %}

**Abstract**

Motivation: The cornea is a layered optical structure in which the epithelium actively remodels in response to the underlying stromal geometry. While the stroma is largely static, the epithelial layer is dynamic and compensatory, adapting to stromal irregularities caused by trauma or refractive surgery. Accurately modeling this remodeling behavior is clinically important, as epithelial compensation can mask stromal abnormalities and influence postoperative outcomes. Existing approaches typically rely on expert-designed analytical or rule-based models calibrated to specific patient cohorts.These models fail to generalize due to patient-specific variability and the complexity of epithelial response mechanisms.

Results: We propose a data-driven framework that models epithelial remodeling as a supervised image-to-image prediction task. Using a U-Net-based architecture, the network takes stromal elevation maps as input and predicts the corresponding anterior (epithelial) elevation map. This formulation allows the model to learn complex, spatially localized remodeling patterns directly from data, without imposing restrictive analytical assumptions. Model outputs are further evaluated using mean curvature analysis to assess anatomical plausibility and relevance beyond raw reconstruction error.

Conclusion: This work introduces a general deep learning framework for predicting corneal epithelial geometry from stromal structure alone, addressing a long-standing gap in corneal biomechanics modeling. By learning epithelial remodeling behavior directly from population-level data, the proposed approach has the potential to generalize across diverse patient cohorts and provide valuable preoperative insights.

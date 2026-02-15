---
layout: page
title: Machine Learning-Based Detection of Keratoconus Using Zernike Polynomials Derived from Corneal Pachymetry Profile
description: An interpretable machine learning framework for keratoconus detection that leverages Zernike polynomial representations of corneal thickness maps to achieve high accuracy, with a special focus on early keratoconus cases.
img: assets/img/Zernike.jpeg
importance: 2
category: Finished
---

{% include figure.html path="assets/img/Zernike.jpeg" title="Zernike-Based Keratoconus Classification" class="img-fluid rounded z-depth-1" %}

**Model:** [https://huggingface.co/spaces/HaidarJomaa/TabNet_Kerato](https://huggingface.co/spaces/HaidarJomaa/TabNet_Kerato)

**Abstract**

Motivation: Keratoconus is a progressive corneal ectatic disorder characterized by localized thinning and biomechanical weakening of the cornea. Early detection is critical for preventing irreversible vision loss, yet most clinical and computational approaches rely predominantly on anterior corneal curvature, which may fail to capture subtle early-stage changes. Corneal pachymetry (thickness) profiles, while biomechanically informative, remain underutilized in automated keratoconus detection despite their ability to summarize structural and material alterations of the cornea.

Results: We propose an interpretable machine learning framework that models keratoconus using corneal thickness maps rather than curvature alone. The pachymetry maps are compactly represented using Zernike polynomials, yielding a 10-dimensional feature vector that captures the dominant spatial modes of corneal thinning. These coefficients act as predefined, physiologically meaningful features tailored to surface deformation analysis. Using these features, we train a TabNet classifier under stratified 5-fold cross-validation. The model achieves perfect classification accuracy for keratoconus versus normal corneas, and maintains strong performance when including subclinical and early-stage cases, reaching approximately 92% F1-score.

Conclusion: This work demonstrates that corneal thickness profiles, when summarized through Zernike polynomial decomposition, provide a powerful and interpretable basis for keratoconus detection. Beyond achieving high performance, the proposed approach enhances clinical interpretability and offers new insights into the biomechanical underpinnings of keratoconus.

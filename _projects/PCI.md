---
layout: page
title: Revisiting the Inferior-Superior (I-S) Value Metric using Machine Learning for Early Detection of Keratoconus
description: A data-driven re-examination of the Inferior–Superior (I–S) index that introduces a posterior curvature-informed metric and leverages machine learning to significantly improve early and subclinical keratoconus detection.
img: assets/img/PCI.jpeg
importance: 3
category: Finished
---

{% include figure.html path="assets/img/PCI.jpeg" title="Machine Learning-Enhanced Keratoconus Detection via Posterior Curvature" class="img-fluid rounded z-depth-1" %}

**Abstract**

Motivation: The Inferior–Superior (I–S) value is a widely used metric for keratoconus screening, computed by sampling curvature values at discrete points along multiple radial axes, averaging these values, and subtracting the superior half from the inferior half. While simple and interpretable, this point-based formulation fails to robustly capture spatially distributed curvature abnormalities, particularly in subclinical disease. Furthermore, clinical workflows continue to prioritize anterior curvature. A key limitation has been the lack of effective feature construction methods for posterior curvature data.

Results: We propose a revised formulation of the I–S metric that replaces single-point radial sampling with sector-based curvature aggregation. Instead of evaluating curvature at isolated points, our method partitions the corneal surface into meaningful sectors. This sector-based representation improves robustness and better captures spatial patterns of posterior corneal deformation. The resulting Posterior Curvature Index (PCI) substantially outperforms traditional Anterior-I–S and Posterior-I–S metrics. In binary classification (keratoconus vs. normal), PCI achieves 97% accuracy compared to 70% for Posterior-I–S and 90% for Anterior-I–S. In three-class classification (normal, subclinical, keratoconus), PCI reaches 89% accuracy, yielding a 47% improvement in F1-score for the subclinical class over Posterior-I–S and a 34% improvement over Anterior-I–S.

Conclusion: This work addresses a fundamental limitation of the traditional I–S metric. Coupled with machine learning, the proposed posterior-curvature-informed index offers a more robust approach to early keratoconus detection.

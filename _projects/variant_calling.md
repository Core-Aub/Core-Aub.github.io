---
layout: page
title: Efficient Variant Calling via 1D Feature Vector Representations
description: A resource-efficient approach to variant calling that replaces 2D pileup image representations with compact 1D feature vectors, aiming to retain high accuracy while reducing computational and memory overhead compared to state-of-the-art deep learning methods.
img: assets/img/VC.jpeg
importance: 3
category: Ongoing
---

{% include figure.html path="assets/img/VC.jpeg" title="Variant Calling Using 1D Feature Vectors" class="img-fluid rounded z-depth-1" %}

**Abstract**

Motivation: Variant calling is a foundational task in genomics, enabling the identification of single nucleotide variants and small insertions/deletions by comparing sequencing reads against a reference genome. Accurate variant detection underpins numerous downstream applications, including disease association studies, population genetics, and clinical diagnostics. Recent state-of-the-art approaches, most notably deep learning-based methods, have achieved impressive accuracy by encoding read pileups as 2D images and applying convolutional neural networks. While effective, this formulation incurs substantial computational, memory, and data preprocessing costs, limiting scalability and accessibility.

Results: We propose an alternative formulation of variant calling that represents local genomic evidence as compact 1D feature vectors rather than 2D images. These vectors encode informative statistics derived from read alignments, base qualities, and so on. By operating directly on structured numerical features, our approach significantly reduces input dimensionality and preprocessing complexity.

Conclusion: This project challenges the prevailing assumption that high-performing variant calling models require 2D image-based representations. By reframing variant calling as a learning problem over carefully designed 1D feature vectors, we offer a more computationally efficient and interpretable alternative that remains compatible with modern deep learning architectures.

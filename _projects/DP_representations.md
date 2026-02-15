---
layout: page
title: Understanding Differential Privacy Through Representation Stability, Utility, and Attack Vulnerability
description: A systematic study of how differential privacy reshapes neural representations in medical deep learning, linking privacy budgets to feature persistence, model utility, and empirical attack success rates.
img: assets/img/DP_rep.jpeg
importance: 2
category: Ongoing
---

{% include figure.html path="assets/img/DP_rep.jpeg" title="Effects of Differential Privacy on Representation Learning" class="img-fluid rounded z-depth-1" %}

**Abstract**

Motivation: Privacy preservation is a central requirement in medical machine learning, where sensitive patient data must be protected against unintended leakage. Differential Privacy (DP) provides formal, mathematically grounded privacy guarantees and has been widely adopted in neuroscience and medical AI. However, most prior work evaluates DP primarily through the privacy–utility tradeoff, focusing on performance degradation as noise increases. This perspective overlooks a critical question: how does differential privacy fundamentally alter the internal representations learned by deep neural networks? Moreover, while DP guarantees are theoretical, real-world threats are driven by concrete attacks such as membership inference, creating a gap between formal privacy budgets and practical risk.

Results: We investigate the effect of varying differential privacy budgets on representation learning in deep neural networks trained on medical data. By analyzing internal feature embeddings across privacy regimes, we study which features remain stable under strong noise injection and which become obscured or suppressed. This enables a qualitative and quantitative characterization of representation robustness under DP. In parallel, we evaluate downstream utility and empirically measure attack success rates, including membership inference attacks, across the same privacy budgets. This results in a direct three-way relationship between privacy budget, model utility, and attack vulnerability, allowing us to map formal privacy guarantees to real-world adversarial risk.

Conclusion: By explicitly connecting privacy budgets to learned feature stability and attack success rates, we provide actionable guidance for practitioners: for a desired performance level, one can estimate the expected privacy protection and residual attack risk. The proposed framework bridges the gap between theoretical DP guarantees and practical security concerns, offering a more interpretable and risk-aware foundation for deploying privacy-preserving deep learning in medical settings.

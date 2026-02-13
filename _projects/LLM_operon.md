---
layout: page
title: Transformer-Based Operon Prediction Using Textual Representations of Gene Pairs
description: A transformer-based method for bacterial operon prediction that frames adjacent gene pairs as a text classification task, enabling robust, cross-species performance using serialized genomic features without reliance on curated networks or extensive annotation.
img: assets/img/LLM.png
importance: 2
category: Finished
---

{% include figure.html path="assets/img/LLM.png" title="Transformer-Based Operon Prediction" class="img-fluid rounded z-depth-1" %}

**Code:** [https://github.com/BasselFakhry/Operons_LLMs](https://github.com/BasselFakhry/Operons_LLMs)

**Abstract**

Motivation: Operons are a fundamental unit of gene regulation in bacteria and can provide valuable insights into genome organization, co-expression, and functional relationships between genes. Computational prediction of operons can support downstream analyses such as pathway reconstruction, comparative genomics, and gene function inference. However, many existing tools rely on structured inputs and curated interaction networks, limiting their applicability to poorly annotated genomes.

Results: We propose a transformer-based approach that reformulates operon prediction as a binary text classification task over adjacent gene pairs. By serializing genomic features—including gene orientation, intergenic distance, GC content, functional annotations, protein families, and conservation—into natural language descriptions, we enable pre-trained language models to perform operon classification using flexible, widely available inputs. Our RoBERTa-based model achieves competitive predictive performance under multiple evaluation settings, including cross-species and leave-one-species-out regimes. Through ablation and inference-time resilience analyses, we demonstrate that sequence-derived and annotation-based features are sufficient for high performance, and that the model remains robust even when key features are missing.

Conclusion: This work introduces a language model-based operon prediction framework that avoids dependence on curated networks and rigid feature engineering pipelines. It offers a flexible and extensible alternative to existing approaches, suitable for large-scale or annotation-limited genomic settings.

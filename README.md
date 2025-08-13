
# Domain-Adversarial Neural Network and Explainable AI for Reducing Tissue-of-Origin Signal in Pan-cancer Mortality Classification

**Authors:**
Cristian Padron-Manrique, Juan José Oropeza Valdez, Osbaldo Resendis-Antonio
**Publication date:** April 14, 2025
**Preprint:** [arXiv:2504.10343](https://arxiv.org/abs/2504.10343)

## Overview

Tissue-of-origin signals dominate pan-cancer gene expression, often overshadowing molecular features associated with patient survival. This hampers the identification of generalizable biomarkers, as models tend to overfit tissue-specific patterns rather than capture survival-relevant signals.

To address this, we propose a **Domain-Adversarial Neural Network (DANN)** trained on **TCGA RNA-seq** data, designed to learn representations less biased by tissue and more focused on mortality prediction. Identifying tissue-independent genetic profiles is key to revealing core cancer programs.

## Methodology

We evaluated the DANN using three complementary strategies:

1. **Standard SHAP**

   * Computed on the original input space and the DANN’s mortality classifier.
   * Interprets gene contributions but remains confounded by tissue bias inherent in SHAP computation.

2. **Unsupervised Activation Manifold**

   * Based on raw hidden-layer activations.
   * Dominated by high-magnitude activations, which mask subtle tissue- and mortality-related signals.

3. **Layer-aware SHAP Manifold**

   * Applies SHAP directly to hidden-layer activations.
   * Produces improved low-dimensional representations of both tissue and mortality signals, independent of activation magnitude.
   * Enables subpopulation stratification and pan-cancer identification of survival-associated genes.

## Key Contributions

* **Bias Mitigation:** Reduces tissue-of-origin signal in pan-cancer mortality classification.
* **Explainability Enhancement:** Introduces a layer-aware SHAP approach to uncover mortality-specific molecular patterns.
* **Biological Insight:** Supports discovery of tissue-independent biomarkers and core cancer pathways relevant to patient survival.



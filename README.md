# ProtoKAN: Integrating Kolmogorov–Arnold Networks into Prototype Learning for Interpretable Image Classification

**Official project repository for ProtoKAN**

> **Code availability:** The source code is not publicly available at this stage. We plan to release the implementation and instructions for reproducing the experiments upon acceptance of the manuscript.

## Overview

ProtoKAN is a prototype-based framework for interpretable fine-grained image classification. It integrates Kolmogorov–Arnold Networks (KAN) into visual part-prototype learning while retaining the *“this looks like that”* reasoning structure.

The framework consists of four main modules:

- **KAN Feature Projection (KFP):** Uses learnable B-spline functions for nonlinear feature projection.
- **KAN-Gated Deformable Matching (KGDM):** Uses a KAN-based gate to modulate offsets for deformable prototype matching.
- **Prototype Context Calibration (PCC):** Calibrates prototype similarity scores using global image context.
- **KAN Prototype Classifier (KAN-PC):** Maps calibrated prototype scores to class logits through nonlinear prototype-level responses, whose contributions can be explicitly aggregated.

## Reported Results

The following Top-1 classification accuracies are reported in the manuscript under the experimental settings described therein.

| Dataset | Top-1 Accuracy |
|:--|--:|
| CUB-200-2011 | **87.4%** |
| Stanford Cars | **89.3%** |

The source code and detailed reproduction instructions will be added to this repository as described in the Code Release section.

## Code Release

The manuscript has not yet been accepted for publication. The source code is therefore not publicly available at present.

Upon acceptance, we plan to update this repository with the implementation, environment requirements, configuration files, and instructions for training and evaluation.

Until the code is released, this repository serves as the official project information page.

## Datasets

Our experiments use the publicly available **CUB-200-2011** and **Stanford Cars** datasets.

Dataset files are not distributed through this repository. Users should obtain the datasets from their respective official sources and follow the applicable terms of use.

## Authors

- Xiongwei Huang (co-first author)
- Prof. Xiaolin Li (co-first author)
- Binbin Chen
- Mingchen Jiang
- Prof. Shiguo Huang (corresponding author)

All authors are affiliated with **Fujian Agriculture and Forestry University, China**.

## Contact

For questions about this project, please contact:

- **Xiongwei Huang:** [huangxw0408@gmail.com](mailto:huangxw0408@gmail.com)
- **Shiguo Huang (corresponding author):** [sghuang@fafu.edu.cn](mailto:sghuang@fafu.edu.cn)

## Citation

A citation entry will be provided once the manuscript is published.

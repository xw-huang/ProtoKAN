# ProtoKAN: Nonlinearizing the Prototype Evidence Flow with Kolmogorov–Arnold Networks for Interpretable Image Classification

**Official project repository for ProtoKAN**

> **Code availability:** The source code is not publicly available at this stage. We plan to release the implementation and instructions for reproducing the experiments upon acceptance of the manuscript.

## Overview

ProtoKAN is a part-prototype network for interpretable fine-grained image classification. It makes the response of each operator in the prototype evidence flow learnable by instantiating three of the four operators with univariate B-spline functions grounded in the Kolmogorov–Arnold representation theorem, and the calibration operator with a context-aware attention mechanism, while preserving the *"this looks like that"* reasoning topology.

The framework consists of four modules:

- **KAN Feature Projection (KFP):** replaces the fixed channel projection with spline-parameterized channel mixing.
- **KAN-Gated Deformable Matching (KGDM):** modulates the predicted deformation offsets with a gate conditioned on global image context.
- **Prototype Context Calibration (PCC):** recalibrates prototype similarities using image-level context.
- **KAN Prototype Classifier (KPC):** replaces the linear head with spline-parameterized evidence aggregation.

## Reported Results

With a ResNet-50 backbone, ProtoKAN reaches the following Top-1 accuracies under the experimental settings described in the manuscript.

| Dataset | Top-1 Accuracy |
|:--|--:|
| CUB-200-2011 | **87.6%** |
| Stanford Cars | **89.5%** |

This is the highest among the compared methods on Stanford Cars and within 0.2 points of the best on CUB-200-2011. An ablation study on a subset of CUB-200-2011 shows that each of the four modules contributes positively and that the full configuration performs best.

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
- Prof.Xiaolin Li (co-first author)
- Binbin Chen
- Mingchen Jiang
- Prof.Shiguo Huang (corresponding author)

All authors are affiliated with **Fujian Agriculture and Forestry University, China**.

## Contact

For questions about this project, please contact:

- **Xiongwei Huang:** [huangxw0408@gmail.com](mailto:huangxw0408@gmail.com)
- **Shiguo Huang (corresponding author):** [sghuang@fafu.edu.cn](mailto:sghuang@fafu.edu.cn)

## Citation

A citation entry will be provided once the manuscript is published.

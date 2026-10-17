---
layout: page
title: Breast cancer detection from mammograms
description: Combining CNN and attention-based (DeiT) image models with patient metadata to detect breast cancer in screening mammograms.
importance: 3
category: masters @ Penn State
---

**Penn State, Jan 2023 to May 2023 (team project with Irfan Tekdir and Akshaya Patil)**

Built a two-step model that classifies screening mammograms from the Kaggle RSNA dataset as cancerous or not. The data is hard to learn from: only about 2% of images show cancer, labels are given per patient across four views, and metadata such as age, breast density and BI-RADS score is often missing.

- **Images.** Converted DICOM scans to grayscale, cropped away non-breast regions and enhanced contrast, then fine-tuned pretrained ResNet-50, ResNet-101 and DenseNet-121 models with focal loss to counter the class imbalance. Concatenating the CC and MLO views of the same breast improved DenseNet-121's AUC-ROC by 30% (from 0.56 to 0.73) at the same 512×256 resolution.
- **Metadata.** Compared XGBoost, random forests and gradient boosting on age, density and BI-RADS, handling missing values by dropping or median imputation, with 10-fold cross-validation. Gradient boosting reached an AUC-ROC of 0.81 with imputed data.
- **Integration.** Added each CNN's predicted cancer probability as a feature in the metadata and trained the tree ensembles on the combined data, reaching an AUC-ROC of about 0.82, 12% higher than the best image-only model (0.73).

The metadata carried most of the signal, and the extreme class imbalance kept precision and recall low. Building on this, I also trained an attention-based vision transformer (DeiT) on the mammograms, and model-based imputation of missing density values was the other proposed next step.

[Project report](https://drive.google.com/file/d/1AFnkoMJ5RzAbXro2cfKgALc56rRoCecU/view?usp=sharing)

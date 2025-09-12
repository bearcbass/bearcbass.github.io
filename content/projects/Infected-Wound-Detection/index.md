---
title: Infected Wound Classification
seo_title: Infected Wound Classification
summary: "An overview of my masters thesis project.  "
description: "The project uses colony forming units (CFUs) as a classification metric for infection, leveraging computer vision and deep learning to analyze wound images."
slug: ml-multiclass-classification
author: bearcbass

date: 2025-08-19T15:55:33-08:00
lastmod: 
expiryDate: 
publishDate: 

feature_image: assets/images/sebas.png
feature_image_alt: "Image alt description"

project types:
  - Machine Learning

techstack:
  - Python
  - PyTorch
  - Labelbox

live_url: 
source_url: https://drive.google.com/file/d/1b0c6nWFWiL0CXI0E0Tmg5p-ruU00a59q/view?usp=sharing

newsletter: false
---

# Deep Learning for Wound Infection Detection

For my master’s thesis at UC Santa Cruz, I developed a deep learning model to classify wound infections from images. The project addressed a critical healthcare challenge: early detection of wound infections, which, if missed, can lead to severe complications like sepsis.

Using a multi-task U-Net architecture, I trained the model on a dataset of 241 wound images labeled with microbiological colony-forming unit (CFU) counts. This labeling method provided an objective standard, unlike most prior work that relied only on clinician judgment.

I tested three training setups:

- **Baseline model with class weighting** – achieved **91.7% accuracy** while correctly identifying most infections.

- **With data augmentation** – improved generalization but became more conservative at higher thresholds.

- **5-fold cross-validation with augmentation** – achieved perfect recall of infected cases at a lower threshold, showing potential for use as a screening tool.

The results showed that my model could catch all infected cases (zero false negatives) under the right threshold, which is critical in medical applications where missing an infection is unacceptable.

While the dataset size limited generalizability, this work highlights how deep learning can support automated, image-based infection screening and lays groundwork for future models trained on larger, more diverse clinical datasets.






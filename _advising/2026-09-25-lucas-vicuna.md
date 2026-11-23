---
title: "Intermediate Representations of Pretrained Models for Efficient Multiple Instance Learning in Histopathological Images"
collection: advising
category: advisor
type: "Master's Thesis (Magíster en Ciencias de la Computación)"
permalink: /advising/2026-09-25-lucas-vicuna
venue: "Universidad Diego Portales, Facultad de Ingeniería y Ciencias"
date: 2026-09-25
period: "2026 – present"
location: "Santiago, Chile"
student: "Lucas Vicuña"
status: "In progress"
---

**Spanish title:** Representaciones intermedias de modelos pre-entrenados para Multiple Instance Learning eficiente en imágenes histopatológicas  
**Student:** Lucas Vicuña  
**Degree:** Master's Thesis (Magíster en Ciencias de la Computación)  
**My Role:** Primary Advisor (Profesor Guía)  
**Institution:** Universidad Diego Portales, Facultad de Ingeniería y Ciencias  
**Location:** Santiago, Chile  
**Period:** 2026 – present  
**Status:** In progress  


### Overview

Computational analysis of histopathological images is limited by the scarcity of detailed annotations, which are costly and require medical expertise. Multiple Instance Learning (MIL) addresses this by splitting each image into instances that share a single image-level label. In most MIL models, however, instances are pixel-space patches, each passed separately through the network, and only the last-layer representation is kept.

This thesis asks whether sub-regions of intermediate feature maps from pretrained networks can replace raw patches as MIL instances, preserving or improving discriminative performance while reducing computational cost. Building on [Zambrano et al. (2022)](/publication/2022-04-18-lowlevel_cnn), which showed that intermediate layers of pretrained CNNs are discriminative without fine-tuning, each tissue image is processed once up to a selected intermediate layer, and the resulting feature map is partitioned into sub-regions that form the MIL instances.

### Methodology

- Evaluation on BreakHis (7,909 breast tumor images from 82 patients, at 40×, 100×, 200×, and 400×), with all splits made strictly at the patient level: a held-out test set and K-fold cross-validation on the development set.
- Attention-based MIL aggregation (soft and gated attention), which also yields interpretable maps of the regions behind each decision.
- A fair comparison against a traditional baseline (last-layer features from pixel-space patches) under the same aggregation, splits, and optimizer, reporting accuracy, precision, recall, and AUC with 95% bootstrap confidence intervals.
- A benchmark of computational cost: time, memory, and floating-point operations.

### Key Technologies

- Multiple Instance Learning with soft and gated attention
- Pretrained CNNs with frozen weights (e.g., ResNet, EfficientNet) and intermediate feature maps
- Dimensionality reduction of feature maps (learned projections and statistical channel selection)
- BreakHis, with PatchCamelyon and BACH as alternative datasets

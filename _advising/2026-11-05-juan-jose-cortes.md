---
title: "Automatic Detection and Grading of Diabetic Retinopathy in High-Resolution Fundus Images"
collection: advising
category: research_practice
type: "Research Practice II (Práctica de Investigación II)"
permalink: /advising/2026-11-05-juan-jose-cortes
venue: "Universidad Diego Portales, Escuela de Informática y Telecomunicaciones"
date: 2026-11-05
period: "Second semester 2026"
location: "Santiago, Chile"
student: "Juan José Cortés"
status: "In progress"
---

**Spanish title:** Detección y gradación automática de retinopatía diabética en retinografías de alta resolución  
**Student:** Juan José Cortés  
**Activity:** Research Practice II (Práctica de Investigación II)  
**My Role:** Supervisor (Profesor Guía)  
**Institution:** Universidad Diego Portales, Escuela de Informática y Telecomunicaciones  
**Location:** Santiago, Chile  
**Period:** Second semester 2026  
**Status:** In progress  


### Overview

Diabetic retinopathy (DR) is a microvascular complication of diabetes and one of the leading causes of preventable blindness in working-age adults. Screening relies on fundus photographs graded on the five-level international ICDR scale, and the deep learning systems already used for screening in Chile still show low specificity in clinical practice, which leads to many unnecessary referrals. Fundus images also pose a technical challenge: they are high-resolution, and the earliest lesions, microaneurysms, cover very few pixels and practically disappear when the whole image is downscaled.

This practice represents each fundus image as a bag of high-resolution patches, an approach known as Multiple Instance Learning (MIL), and compares it with whole-image baselines built on classical image processing features and on a pretrained convolutional network.

### Objectives

- Preprocess fundus images and build two whole-image baselines: classical image processing features, and a pretrained convolutional network.
- Implement the bag-of-patches representation with classical features and with convolutional features combined through an attention mechanism (attention-MIL), whose weights give an interpretable map of the patches behind each decision.
- Evaluate all methods under a single rigorous protocol, with confidence intervals and paired comparisons against the baseline.
- Analyze errors, model interpretability, and generalization to a second dataset without retraining.
- Propose the dataset and problem formulation for a subsequent thesis.

### Key Technologies

- Multiple Instance Learning with attention (attention-MIL)
- Classical image processing: field-of-view masking, CLAHE, multi-scale morphological top-hat filters
- EfficientNet-B0 pretrained on ImageNet
- IDRiD dataset, part B (516 fundus images of 4288 × 2848 pixels)
- Python, OpenCV, scikit-learn, and PyTorch, with GitLab continuous integration for reproducibility

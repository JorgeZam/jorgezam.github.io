---
title: "A 3D Iris Scanner From a Single Image Using Convolutional Neural Networks"
collection: publications
category: manuscripts
permalink: /publication/2020-05-22-3d-iris-scanner-cnn
excerpt: 'A single-image 3D iris reconstruction method based on a depth-estimation CNN, trained on synthetic and real iris datasets, that improves recognition performance by 48% over the standard 2D iris code.'
date: 2020-05-22
venue: 'IEEE Access'
paperurl: 'https://ieeexplore.ieee.org/document/9097841'
bibtexurl: 'https://jorgezam.github.io/files/3d_iris_scanner_cnn.bib'
citation: 'D. P. Benalcazar, <b>J. E. Zambrano</b>, D. Bastias, C. A. Perez and K. W. Bowyer, &quot;A 3D Iris Scanner From a Single Image Using Convolutional Neural Networks,&quot; in <i>IEEE Access</i>, vol. 8, pp. 98584-98599, 2020, doi: 10.1109/ACCESS.2020.2996563.'
---

A 3D model of the human iris adds an extra degree of freedom to iris recognition, helping identify people in larger databases even when only a portion of the iris is available. This work develops a 3D iris scanner that reconstructs a 3D iris model from a **single 2D image** using a depth-estimation Convolutional Neural Network. To train and evaluate the method, we built a dataset of 26,520 real iris images from 120 subjects and a synthetic dataset of 72,000 iris images with aligned depthmaps. The proposed approach was validated against step-pyramid 3D-printed models, synthetic test images, and OCT scans of both eyes of a subject. A 3D rubber sheet generated from the reconstructed iris model improved iris recognition performance by **48%** over the standard 2D iris code. Additional contributions include reducing the acquisition and processing time and simplifying the image acquisition system.

## How to cite

```bibtex
@article{benalcazar20203diris,
  author    = {Benalcazar, Daniel P. and Zambrano, Jorge E. and Bastias, Diego and Perez, Claudio A. and Bowyer, Kevin W.},
  journal   = {IEEE Access},
  title     = {A {3D} Iris Scanner From a Single Image Using Convolutional Neural Networks},
  year      = {2020},
  volume    = {8},
  pages     = {98584--98599},
  doi       = {10.1109/ACCESS.2020.2996563}
}
```

---
title: "Iris Recognition Using Low-Level CNN Layers Without Training and Single Matching"
collection: publications
category: manuscripts
permalink: /publication/2022-04-18-iris-recognition-low-level-cnn
excerpt: 'A deep-learning approach to iris recognition that uses features from the low-level layers of pretrained CNNs without further training, combined with bit-shifting for robustness against pupil dilation.'
date: 2022-04-18
venue: 'IEEE Access'
paperurl: 'https://ieeexplore.ieee.org/document/9755923'
# bibtexurl: 'https://jorgezam.github.io/files/iris_lowlevel_cnn.bib'
citation: '<b>J. E. Zambrano</b>, D. P. Benalcazar, C. A. Perez and K. W. Bowyer, &quot;Iris Recognition Using Low-Level CNN Layers Without Training and Single Matching,&quot; in <i>IEEE Access</i>, vol. 10, pp. 41276-41286, 2022, doi: 10.1109/ACCESS.2022.3166910.'
---
This work proposes an iris recognition method that leverages features extracted from the low-level layers of pretrained convolutional neural networks, without requiring additional training on iris data. The approach incorporates a bit-shifting strategy to improve robustness against pupil dilation, a known challenge in iris biometrics. Single-matching evaluation on standard iris databases demonstrates competitive recognition performance with reduced computational cost. DOI: [10.1109/ACCESS.2022.3166910](https://doi.org/10.1109/ACCESS.2022.3166910)

## Abstract  
Iris is one of the most accurate biometrics. This has led to the successful development of large-scale applications. However, with population growth, and new international applications, datasets are constantly increasing in size, requiring more robust and faster methods. Many descriptors and feature extractors have been developed to extract features that represent the iris biometric pattern. Most of them have been designed by human experts and require a bit-shifting process to increase their robustness to eye rotations, at the expense of increased matching time. We propose a fast iris recognition method that requires a single matching operation and is based on pre-trained image classification models as feature extractors. Our approach uses the filters of the first layers from Convolutional Neural Networks as feature extractors and does not require fine-tuning for new datasets. Since our selected features extracted from convolutional layers encode the iris surface, they have the advantage of not being restricted to specific spatial positions. Thus, it is not necessary to perform a bit-shifting process in the matching stage, eliminating a significant number of computations. Additionally, to mitigate the effect produced by the mask border in rubber-sheet images, we propose filtering the feature map tensors by masking their channels and selecting the most relevant features. Our method was assessed on the publicly available datasets CASIA Iris Lamp and CASIA Iris Thousand, and showed significant improvement both in accuracy and in matching time.

## How to cite

```bibtex
@article{zambrano2022irislowlevel,
  author    = {Zambrano, Jorge E. and Benalcazar, Daniel P. and Perez, Claudio A. and Bowyer, Kevin W.},
  journal   = {IEEE Access},
  title     = {Iris Recognition Using Low-Level CNN Layers Without Training and Single Matching},
  year      = {2022},
  volume    = {10},
  pages     = {41276--41286},
  doi       = {10.1109/ACCESS.2022.3166910}
}
```

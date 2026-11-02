---
title: "Learning from Less: Pose-Balanced Sampling for High-Performance Face Recognition"
collection: publications
selected: true
category: manuscripts
permalink: /publication/2026-11-02-pose_balanced_sampling
excerpt: 'A pose-balanced sampling strategy that builds a compact face recognition training subset by retaining an equal number of frontal and profile images per identity, preserving most large-pose verification accuracy while greatly reducing training time.'
date: 2026-11-02
venue: 'Sensors'
paperurl: 'https://www.mdpi.com/1424-8220/26/21/6937'
bibtexurl: 'https://jorgezam.github.io/files/pose_balanced_sampling.bib'
citation: 'J. I. Pilataxi, <b>J. E. Zambrano</b>, R. Guamán-Rivera and R. Olivares, &quot;Learning from Less: Pose-Balanced Sampling for High-Performance Face Recognition,&quot; in <i>Sensors</i>, vol. 26, no. 21, p. 6937, 2026, doi: 10.3390/s26216937.'
---
This work proposes a pose-balanced sampling strategy that builds a compact face recognition training subset by conditioning selection on the per-identity head-pose distribution. Yaw angles are estimated with 6DRepNet, and an equal number of frontal and profile images are retained for every identity. Applied to MS1Mv3, the strategy yields MS1Mv3-FP, a subset of 547,202 images (10.7% of the original) covering 78.5% of the identities. An SE-ResNet100 trained from scratch on this subset with the ArcFace loss reaches up to 98.73%, 93.23%, and 94.74% verification accuracy on CFP-FP, CPLFW, and VGG2-FP, within 0.30, 0.70, and 0.86 percentage points of the same network trained on the complete dataset, while reducing training time from more than 100 h to approximately 11 h on a single GPU. Frontal–frontal verification accuracy is largely preserved, whereas age-gap verification degrades.
## How to cite
```bibtex
@article{pilataxi2026posebalanced,
  author    = {Pilataxi, Jhon I. and Zambrano, Jorge E. and Guam{\'a}n-Rivera, Robert and Olivares, Rodrigo},
  journal   = {Sensors},
  title     = {Learning from Less: Pose-Balanced Sampling for High-Performance Face Recognition},
  year      = {2026},
  volume    = {26},
  number    = {21},
  pages     = {6937},
  doi       = {10.3390/s26216937}
}
```

---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Ph.D. in Electrical Engineering from Universidad de Chile, specialized in **Image Processing** and **Artificial Intelligence**. My research lies at the intersection of *deep learning*, image processing, and data science. I completed my undergraduate studies in Ecuador, earning a degree in Electronic Engineering with a specialization in Instrumentation.

I am currently a faculty member at **Universidad Diego Portales**.

## Current Research

My current research focuses on weakly supervised learning applied to the detection of irregularities in histopathological tissue. Specifically, I work with Multiple Instance Learning (MIL) frameworks for Whole Slide Image (WSI) analysis, aiming to identify pathological patterns without requiring exhaustive pixel-level annotations.

## Selected Publications

{% assign selected_pubs = site.publications | where: "selected", true | sort: "date" | reverse %}
{% for post in selected_pubs %}
- {{ post.citation }} [[Details]]({{ post.url }})
{% endfor %}

[See all publications: ](/publications/)

## Doctoral stage and research

During my doctoral studies I specialized in biometric modeling using convolutional neural networks (CNNs). I have participated in the **FONDECYT 1231675** and **1191610** projects, focused on facial biometrics, 3D iris modeling, and deep learning, as well as in the **IMPACT Basal Project (FB210024)**, where I investigated the use of *deep learning* for biomedical image analysis, including the detection of psychiatric disorders from extracellular vesicles.

## Postdoctoral stage

During my postdoctoral stage, a key contribution was my participation in the **FONDEF ID24I10408** project, where I developed intelligent systems for the detection of illegal products through the multimodal integration of text and image.

## Teaching and collaboration

I have over six years of teaching experience in courses on **programming**, **signals and systems**, **image processing**, and **artificial intelligence**, and I maintain active scientific collaboration networks both nationally and internationally.


## Contact

For collaborations or inquiries: [jorge.zambrano@mail.udp.cl](mailto:jorge.zambrano@mail.udp.cl)

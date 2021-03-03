---
layout: page
title: Colorectal Polyps Characterization
background: grey
cat: health


caption:
  title: Colorectal Polyps Characterization
  #subtitle: Illustration
  thumbnail: assets/img/portfolio/unitopatho-thumbnail_o.jpg
---

# Colorectal Polyps Characterization

The use-case will focus on gastrointestinal pathology, specifically colon biopsies: these particular
samples represent a cornerstone activity for any surgical pathology laboratory. Differential diagnosis
includes a limited number of entities, mostly neoplastic (i.e. adenomas) and more rarely inflammatory.
Histopathological characterization of colorectal polyps by pathologists is the major tool for deciding
the following clinical/therapeutic management of patients. The histological slides contain histological
sections of the biological specimens stained with hematoxylin and eosin (H&E); H&E are chemical
substances used to achieve visible colour contrast, allowing morphological diagnosis based on
pattern recognition and assessment of specific features.
Deep-learning is being investigated by the scientific community as a possible tool to cut the overall
laboratory workload, but also to improve the diagnostic and prognostic efficacy of histological
examination. In this use case, some recent results in colorectal polyps classification will be
taken into account and, if possible, used as a benchmark and independently validated.
The medical experts participating to the use case selected six different classes for automatic
classification which represent the most common diagnoses and lead to different patients’
management:

- Normal tissue (NORM)
- Hyperplastic polyp (HP)
- Tubular Adenoma, high-grade dysplasia (TA.HG)
- Tubular Adenoma, low-grade dysplasia (TA.LG)
- Tubulovillous Adenoma, high-grade dysplasia (TVA.HG)
- Tubulovillous Adenoma, low-grade dysplasia (TVA.LG)

<div class="row" style="padding: 20px; padding-left: 50px; padding-right: 50px">
  <img class="img-fluid" src="assets/img/portfolio/unitopatho/unitopatho.png"/>
</div>

The Pathology Unit of UNITO will provide a labeled set of whole-slide biopsy images that will be
exploited by machine learning experts in the team for models training and testing on DeepHealth ODH
platform (PF5). {%cite barbano2021unitopatho perlo2021dysplasia unitopatho %}

**Data**

You can access the dataset at <a href='https://ieee-dataport.org/open-access/unitopatho'>https://ieee-dataport.org/open-access/unitopatho</a>

**References**:

{% bibliography --cited %}

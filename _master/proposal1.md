---
title: GAN-based augmentation of wholeslides images for colorectal polyps characterization
type: Research
image: assets/img/proposals/gan_hp.png
alt: Shirts on a hanger
contact:
  - carlo.barbano@unito.it
  - enzo.tartaglione@unito.it
  - marco.grangetto@unito.it
  - eidoslab@di.unito.it
---

Histopathological characterization of colorectal polyps allows to tailor patients’ management and follow up with the ultimate aim of avoiding or promptly detecting an invasive carcinoma. Colorectal polyps characterization relies on the histological analysis of tissue samples to determine the polyps malignancy and dysplasia grade. Deep neural networks achieve outstanding accuracy in medical patterns recognition, however they require large sets of annotated training images.

The aim of this thesis is to employ **generative models** (i.e GANs) for the generation of synthetic tissue patches and to assess the potential benefits when used in conjuction with real-world data, for predicting the dysplasia grade (*i.e. how likely the tissue is to develop into cancer*). The generation process will start from segmentation maps, in order to allow for finer control over the synthesized images.

**References:**

[1] L. Hou, A. Agarwal, D. Samaras, T. M. Kurc, R. R. Gupta and J. H. Saltz, "Robust Histopathology Image Analysis: To Label or to Synthesize?," 2019 IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), Long Beach, CA, USA, 2019, pp. 8525-8534, doi: 10.1109/CVPR.2019.00873.

[2] Barbano, C. A., Perlo, D., Tartaglione, E., Fiandrotti, A., Bertero, L., Cassoni, P., & Grangetto, M. (2021). UniToPatho, a labeled histopathological dataset for colorectal polyps classification and adenoma dysplasia grading. arXiv preprint arXiv:2101.09991.

[3] Luca Bertero, Carlo Alberto Barbano, Daniele Perlo, Enzo Tartaglione, Paola Cassoni, Marco Grangetto, Attilio Fiandrotti, Alessandro Gambella, Luca Cavallo. (2021). UNITOPATHO. IEEE Dataport. https://dx.doi.org/10.21227/9fsv-tm25

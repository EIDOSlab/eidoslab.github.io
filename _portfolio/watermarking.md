---
layout: page
title: Watermarking deep neural networks
background: grey
cat: deep learning


caption:
  title: Watermarking deep neural networks
  #subtitle: Graphic Design
  thumbnail: assets/img/portfolio/valley_watermark.png
---

# Delving in the loss landscape to embed robust watermarks into neural networks

In the last decade the use of artificial neural networks (ANNs) in many fields like image processing or speech recognition has become a common practice because of their effectiveness to solve complex tasks. However, in such a rush, very little attention has been paid to security aspects. In this work we explore the possibility to embed a watermark into the ANN parameters.
We exploit model redundancy and adaptation capacity to lock a subset of its parameters to carry the watermark sequence. The watermark can be extracted in a simple way to claim copyright on models but can be very easily attacked with model fine-tuning.
To tackle this culprit we devise a novel watermark aware training strategy. We aim at delving into the loss landscape to find an optimal configuration of the parameters such that we are robust to fine-tuning attacks towards the watermarked parameters.
Our experimental results on classical ANN models trained on well-known MNIST and CIFAR-10 datasets show that the proposed approach makes the embedded watermark robust to fine-tuning and compression attacks.

[![Video: Delving in the loss landscape to embed robust watermarks into neural networks](https://img.youtube.com/vi/coDIgb3n_LA/0.jpg)](https://youtu.be/coDIgb3n_LA "Video: Delving in the loss landscape to embed robust watermarks into neural networks")

**References:**

[1] Tartaglione, E., Grangetto, M., Cavagnino, D. & Botta, M. (2021). Delving in the loss landscape to embed robust watermarks into neural networks. International Conference on Pattern Recognition.

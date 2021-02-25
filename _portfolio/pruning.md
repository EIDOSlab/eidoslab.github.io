---
layout: page
title: Pruning
background: grey
cat: deep learning

caption:
  title: Pruning
  #subtitle: Website Design
  thumbnail: assets/img/portfolio/structured_pruning.png
---

# Pruning deep neural networks

Deep Neural Networks (DNNs) can solve challenging tasks thanks to complex stacks of (convolutional) layers with millions of learnable parameters. DNNs are however challenging to deploy in scenarios where memory is limited (e.g.,  mobile  devices),  since  their  memory  footprint  grows  linearly  with  the  number  of  parameters.  A  number  of strategies have been proposed to tackle this issue, including ad-hoc topology designs, parameter quantization and parameter  pruning.  Parameter pruning consists  in  dropping  synapses  between  neurons,  i.e.  setting  to  zero  part  of the  entries  in  the  matrices  representing  the  connections  between  layers.  Concerning  the  choice  of  the  parameters to prune, a number of different approaches have been proposed. Let us define the sensitivity of a parameter as the derivative of the network output(s) with respect to the parameter. It was shown that parameters with small sensitivity can be pruned from the topology with negligible impact  on  the  network  performance,  outperforming  approaches  based  on  norm  minimization.  Concerning  the network topology resulting from pruning, two different classes of strategies can be identified.

* **Unstructured**  strategies aim  at  maximizing  the  pruning  ratio,  i.e.  the  number  of  parameters  pruned  from the  network,  regardless  of  the  resulting  topology.  For  example,  LOBSTER  (LOss  Based  SensitiviTyRegularization)  is  a  loss-based  regularizer  that  drives  some  but  not  all  parameters  towards  zero.  It  shrinks parameters for which the loss derivative is small, such that many parameters are first driven towards zero and then  pruned  with  a  threshold  mechanism.  In  a  number  of  scenarios,  this  method  yields  competitive  results in  terms  of  pruning  ratio.  The  resulting  connection  matrices  are  however  randomly  sparse,  i.e.  they  have  no structure. Representing sparse matrices in a memory efficient format is a non-trivial problem, thus high pruning ratios do not necessarily translate into reduced memory footprints.

* **Structured**  strategies aim  at  pruning  parameters  from  the  network  yet  with  a  constraint  on  the  resulting topology.  For  example  SeReNe  (Sensitivity-based  Regularization  of  Neurons) is  a  method  for  learning sparse  topologies  with  a  structure,  exploiting  neural  sensitivity  as  a  regularizer.  Here,  the  sensitivity  of  a neuron  is  defined  as  the variation  of  the  network  output  with  respect  to  the  variation  of  the  activity  of  the neuron.  The  lower  the  sensitivity  of  a  neuron,  the  less  the  network  output  is  perturbed  if  the  neuron  output changes. This term is included in the cost function as a regularization term: in such way, SeReNe is able to prune entire neurons at the cost of a somewhat lower pruning ratio.

**References:**

[1] Tartaglione, E., Lepsøy, S., Fiandrotti, A., & Francini, G. (2018). Learning Sparse Neural Networks via Sensitivity-Driven Regularization. NeurIPS.

[2] Tartaglione, Enzo, Andrea Bragagnolo, and Marco Grangetto. "Pruning artificial neural networks: a way to find well-generalizing, high-entropy sharp minima." International Conference on Artificial Neural Networks. Springer, Cham, 2020.

[3] Tartaglione, E., Bragagnolo, A., Odierna, F., Fiandrotti, A., & Grangetto, M. (2021). SeReNe: Sensitivity based Regularization of Neurons for Structured Sparsity in Neural Networks. arXiv preprint arXiv:2102.03773.

[4] Tartaglione, E., Bragagnolo, A., Fiandrotti, A., & Grangetto, M. (2020). LOss-Based SensiTivity rEgulaRization: towards deep sparse neural networks. arXiv preprint arXiv:2011.09905.

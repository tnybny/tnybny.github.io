---
title: 'What I read'
date: 2020-11-01
permalink: /posts/2020/11/What-I-read/
tags:
  - reading list
---

This is a list of select research works that I've read and really like from most to least recent, much like a communication of my stream of consciousness when it comes to research. I would like to think that I could have collborated to write some of these and it is my dream that one day I might produce works like these.


1. [CoordConv](https://arxiv.org/pdf/1807.03247.pdf) in NIPS 2018: brilliant exposition of a curios way in which ConvNets fail and a balatantly simple solution to allow a conv kernel to be aware of it's position in terms of pixel coordinates. Note that this paper weirdly has translation _invariance_ mixed up with translation _equivarance_ a lot. 
1. [SOLO](https://arxiv.org/pdf/1912.04488.pdf%5d%5b2019.pdf) and[SOLOv2](https://arxiv.org/pdf/2003.10152.pdf) on ArXiV 2020: Simple and elegant idea of segmenting instances of objects by separating out in channels the mask predictions by location in image and size; improved in the following work by dynamic convolutions and a fast Matrix NMS scheme.
1. [DETR](https://arxiv.org/pdf/2005.12872.pdf) in ECCV 2020: Object detection with Transformer networks by performing directly fixed set prediction, without the need for RPNs and NMS. 
1. [3D pose estimation with 2D marginal heatmaps](https://arxiv.org/pdf/1806.01484.pdf) in WACV 2019. A beautiful alternative to representing 3D pose ground truth with the memory and computation heavy volumetric heatmaps. 
1. [Deconvolution and checkerboard artifacts](https://distill.pub/2016/deconv-checkerboard/).
1. [Spatial Pyramid Pooling](https://engineering.case.edu/centers/ccipd/system/files/Xiangxue_Spatial%20Pyramid%20Pooling%20....pdf) in TPAMI 2015.
1. [Batch renormalization](http://papers.nips.cc/paper/6790-batch-renormalization-towards-reducing-minibatch-dependence-in-batch-normalized-models.pdf) from NIPS 2017.

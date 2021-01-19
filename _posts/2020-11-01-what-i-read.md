---
title: 'What I read'
date: 2020-11-01
permalink: /posts/2020/11/What-I-read/
tags:
  - reading list
---

This is a list of select research works that I've read and really like from most to least recent, much like a communication of my stream of consciousness when it comes to research. I would like to think that I could have collborated to write some of these and it is my dream that one day I might produce works like these.


### 2020
1. [CoordConv](https://arxiv.org/pdf/1807.03247.pdf) in NIPS 2018: brilliant exposition of a curios way in which ConvNets fail and a balatantly simple solution to allow a conv kernel to be aware of it's position in terms of pixel coordinates. Note that this paper weirdly has translation _invariance_ mixed up with translation _equivarance_ a lot. 
1. [SOLO](https://arxiv.org/pdf/1912.04488.pdf%5d%5b2019.pdf) and [SOLOv2](https://arxiv.org/pdf/2003.10152.pdf) on ArXiV 2020: Simple and elegant idea of segmenting instances of objects by separating out in channels the mask predictions by location in image and size; improved in the following work by dynamic convolutions and a fast Matrix NMS scheme.
1. [A Metric Learning Reality Check](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123700681.pdf) in ECCV 2020: Through benchmark and comparison on deep metric learning research over the past few years, exposing flaws in experimental methodology of several of them.
1. [What Matters in Unsupervised Optical Flow](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123470545.pdf) in ECCV 2020: A thorough study on the different losses, occlusion handling and smoothness regularization strategies in optical flow learning, leading to a new and simple unsupervised optical flow technique that sets new sota in multiple areas.
1. [DETR](https://arxiv.org/pdf/2005.12872.pdf) in ECCV 2020: Object detection with Transformer networks by performing directly fixed set prediction, without the need for RPNs and NMS. 
1. [3D pose estimation with 2D marginal heatmaps](https://arxiv.org/pdf/1806.01484.pdf) in WACV 2019: A beautiful alternative to representing 3D pose ground truth with the memory and computation heavy volumetric heatmaps.
1. [Associative Embeddings](https://papers.nips.cc/paper/2017/file/8edd72158ccd2a879f79cb2538568fdc-Paper.pdf) in NIPS 2017: A way to supervise networks for simultaneous detection and grouping.
1. [Transformers for Image Recognition](https://papers.nips.cc/paper/2017/file/8edd72158ccd2a879f79cb2538568fdc-Paper.pdf) on arXiV 2020: The first successful application of a Transformer directly on images, by breaking them down into sequences of image patches, for recognition tasks. 

### 2019
1. [Domain Adversarial Training of Neural Networks](https://www.jmlr.org/papers/volume17/15-189/15-189.pdf) at JMLR 2017: Elegant idea to use gradient ascent on a "domain discriminator head" enabled by a gradient reversal layer to learn domain invaraint features.
1. [Sampling Matters in Deep Embedding Learning](https://openaccess.thecvf.com/content_ICCV_2017/papers/Wu_Sampling_Matters_in_ICCV_2017_paper.pdf) at ICCV 2017: A study on embeddings for metric learning, emphasizing the importance of training data sampling for learning good embeddings. Also proposes a simple margin-based metric learning loss.
1. [Rethinking the Inception Architecture for Computer Vision](https://openaccess.thecvf.com/content_cvpr_2016/papers/Szegedy_Rethinking_the_Inception_CVPR_2016_paper.pdf) at CVPR 2016: I actually like this paper most for something they only very briefly touch upon, the concept of label smoothing regularization. LSR is a way to regularize classifiers by adding noise to the class probability targets in the cross-entropy loss. By preventing the correct class logit from becoming much larger than all other logits, it makes the model more adaptable.  

### pre 2018
1. [Deconvolution and checkerboard artifacts](https://distill.pub/2016/deconv-checkerboard/).
1. [Spatial Pyramid Pooling](https://engineering.case.edu/centers/ccipd/system/files/Xiangxue_Spatial%20Pyramid%20Pooling%20....pdf) in TPAMI 2015.
1. [Batch renormalization](http://papers.nips.cc/paper/6790-batch-renormalization-towards-reducing-minibatch-dependence-in-batch-normalized-models.pdf) from NIPS 2017.

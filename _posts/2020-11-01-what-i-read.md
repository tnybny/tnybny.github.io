---
title: 'Technical reading'
date: 2020-11-01
permalink: /posts/2020/11/What-I-read/
tags:
  - reading list
---

This is a list of select research works that I've read and like from most to least recently read, much like a communication of my stream of consciousness. I would like to think that I could have collaborated to write some of these and it is my dream that one day I might produce works like these.

### 2024
1. [Map Learning with Lane Segment Perception for Autonomous Driving](https://arxiv.org/abs/2312.16108) at ICLR 2024: A DETR-based approach for detecting lane segments and their relationships for real-time map learning. 
2. [Center-based 3D Object Detection and Tracking](https://arxiv.org/abs/2006.11275) at CVPR 2021: Representing 3D objects as points using a keypoint heatmap detection scheme.
3. [BEVFusion: Multi-Task Multi-Sensor Fusion with Unified Bird's-Eye View Representation](https://arxiv.org/abs/2205.13542) at ICRA2023: LiDAR + Camera fusion in the Bird's Eye View Representation space for autonomous driving tasks.
4. [BEVFormer: Learning Bird's-Eye-View Representation from Multi-Camera Images via Spatiotemporal Transformers](https://arxiv.org/abs/2203.17270) at TPAMI 2024: Using BEV-space queries and a transformer to project image features into the BEV space
5. [PETRv2: A Unified Framework for 3D Perception from Multi-Camera Images](https://arxiv.org/abs/2206.01256) at ICCV 2023: Extended the 3D positional embedding in PETR to temporal modeling and task-specific queries for autonomous driving tasks.

### 2023
1. [Boundary Loss for Highly Unbalanced Segmentation](https://proceedings.mlr.press/v102/kervadec19a.html) at PMLR 2019: A loss function that takes the form of a distance metric over on the space of contours instead of regions, allowing application on highly unbalanced segmentation tasks with relatively stable training.
2. [Generalised Dice Overlap as a Deep Learning Loss Function for Highly Unbalanced Segmentations](https://arxiv.org/abs/1707.03237) at MICCAI 2017: Generalizes the Dice loss with class re-balancing properties through weighting for highly unbalanced segmentation.
3. [Masked-attention Mask Transformer for Universal Image Segmentation](https://arxiv.org/abs/2112.01527) at CVPR 2022: Using a mask to constrain cross-attention within predicted mask regions for dense output prediction tasks, where learnable queries serve as mask proposals (akin to region proposals).

### 2022
1. [Uncertainty Weighted Losses](https://arxiv.org/abs/1705.07115) at CVPR 2018: Simple scheme to learn loss weights in a multi-task framework in a principled manner.
2. [GAN-supervised Dense Visual Alignment](https://openaccess.thecvf.com/content/CVPR2022/papers/Peebles_GAN-Supervised_Dense_Visual_Alignment_CVPR_2022_paper.pdf) at CVPR 2022: Really cool way to use GANs for image congealing, with applications in augmented reality and image editing. They jointly optimize their loss with respect to both a transformation given by a spatial transformer network and a latent code that represents pose.
3. [End-to-End Multi-Person Pose Estimation with Transformers](https://openaccess.thecvf.com/content/CVPR2022/html/Shi_End-to-End_Multi-Person_Pose_Estimation_With_Transformers_CVPR_2022_paper.html) at CVPR 2022: This hits home for me because it's very closely related to something I worked on at Wrnch. It uses the hungarian set-based loss and output positional encodings that DETR suggests to perform for the first time fast fully-differentiable multi-person pose estimation.
4. [Formal Algorithms For Transformers](https://arxiv.org/abs/2207.09238) on ArXiV 2022. Excellent mathematically precise overview of transformer architectures.
5. [Learning Image Representations with a Deformable Grid](https://arxiv.org/abs/2008.09269) at ECCV 2020: Representing images on a deformed grid to better align with high-frequency image content. One reason to be excited about this is the ability to make a prediction at lower resolution which translates without sub-pixel error to higher resolution.
6. [Aligning Semantic Segmentation Maps with Implicit Neural Representations](https://arxiv.org/abs/2206.08655) at ECCV 2022:  The use of implicit neural representations to align features at different levels of an upsampling pyramid and produce segmentation maps at arbitrary resolution. This work is related to Defgrid learning (paper above) in that they both propose strategies that are helpful for image representation at lower resolution, saving compute costs and at the same time having the potential to be more precise.
7. [Pix2PixHD](https://openaccess.thecvf.com/content_cvpr_2018/papers/Wang_High-Resolution_Image_Synthesis_CVPR_2018_paper.pdf) at CVPR 2018: Application of conditional GANs for image synthesis from semantic label maps.


### 2021
1. "Tutorial: Pay Attention to What You Need: Do Structural Priors Still Matter in the Age of Billion Parameter Models?" at NIPS 2021: General principles to bring structure to deep learning systems, partly inspired by Daniel Kahneman's Thinking Fast and Slow.
2. [Masked Autoencoders are Scalable Vision Learners](https://arxiv.org/abs/2111.06377) at CVPR 2022: Presents a new self-learning based pre-training method that works surprisingly well for Transformer models in vision tasks.
3. [Robustness of Vision Transformers to occlusions](https://proceedings.neurips.cc/paper/2021/file/c404a5adbf90e09631678b13b05d9d7a-Paper.pdf) at NIPS 2021: A revealing set of experiments that show that vision transformers are curiously more robust to occlusions when compared to ConvNets.
4. [Spectral Norm for GAN training](https://proceedings.neurips.cc/paper/2021/file/4ffb0d2ba92f664c2281970110a2e071-Paper.pdf) at NIPS 2021: A study on why spectral normalization has been successful in stabilizing GAN training.
5. [Knowledge Distillation for Object Detection](https://arxiv.org/pdf/2103.02340) at CVPR 2021: A knowledge distillation scheme for object detection that is based on distilling information in regions of most disagreement between teacher and student.

### 2020
1. [CoordConv](https://arxiv.org/pdf/1807.03247.pdf) in NIPS 2018: brilliant exposition of a curios way in which ConvNets fail and a balatantly simple solution to allow a conv kernel to be aware of it's position in terms of pixel coordinates. Note that this paper weirdly has translation _invariance_ mixed up with translation _equivarance_ a lot. 
1. [SOLO](https://arxiv.org/pdf/1912.04488.pdf%5d%5b2019.pdf) and [SOLOv2](https://arxiv.org/pdf/2003.10152.pdf) on ArXiV 2020: Simple and elegant idea of segmenting instances of objects by separating out in channels the mask predictions by location in image and size; improved in the following work by dynamic convolutions and a fast Matrix NMS scheme.
1. [A Metric Learning Reality Check](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123700681.pdf) at ECCV 2020: Through benchmark and comparison on deep metric learning research over the past few years, exposing flaws in experimental methodology of several of them.
1. [What Matters in Unsupervised Optical Flow](https://www.ecva.net/papers/eccv_2020/papers_ECCV/papers/123470545.pdf) at ECCV 2020: A thorough study on the different losses, occlusion handling and smoothness regularization strategies in optical flow learning, leading to a new and simple unsupervised optical flow technique that sets new sota in multiple areas.
1. [DETR](https://arxiv.org/pdf/2005.12872.pdf) at ECCV 2020: Object detection with Transformer networks by performing directly fixed set prediction, without the need for RPNs and NMS. 
1. [3D pose estimation with 2D marginal heatmaps](https://arxiv.org/pdf/1806.01484.pdf) at WACV 2019: A beautiful alternative to representing 3D pose ground truth with the memory and computation heavy volumetric heatmaps.
1. [Associative Embeddings](https://papers.nips.cc/paper/2017/file/8edd72158ccd2a879f79cb2538568fdc-Paper.pdf) at NIPS 2017: A way to supervise networks for simultaneous detection and grouping.
1. [Transformers for Image Recognition](https://papers.nips.cc/paper/2017/file/8edd72158ccd2a879f79cb2538568fdc-Paper.pdf) on arXiV 2020: The first successful application of a Transformer directly on images, by breaking them down into sequences of image patches, for recognition tasks. 

### 2019
1. [Domain Adversarial Training of Neural Networks](https://www.jmlr.org/papers/volume17/15-189/15-189.pdf) at JMLR 2017: Elegant idea to use gradient ascent on a "domain discriminator head" enabled by a gradient reversal layer to learn domain invariant features.
1. [Sampling Matters in Deep Embedding Learning](https://openaccess.thecvf.com/content_ICCV_2017/papers/Wu_Sampling_Matters_in_ICCV_2017_paper.pdf) at ICCV 2017: A study on embeddings for metric learning, emphasizing the importance of training data sampling for learning good embeddings. Also proposes a simple margin-based metric learning loss.
1. [Rethinking the Inception Architecture for Computer Vision](https://openaccess.thecvf.com/content_cvpr_2016/papers/Szegedy_Rethinking_the_Inception_CVPR_2016_paper.pdf) at CVPR 2016: I actually like this paper most for something they only very briefly touch upon, the concept of label smoothing regularization. LSR is a way to regularize classifiers by adding noise to the class probability targets in the cross-entropy loss. By preventing the correct class logit from becoming much larger than all other logits, it makes the model more adaptable.  

### pre 2018
1. [Deconvolution and checkerboard artifacts](https://distill.pub/2016/deconv-checkerboard/).
1. [Spatial Pyramid Pooling](https://engineering.case.edu/centers/ccipd/system/files/Xiangxue_Spatial%20Pyramid%20Pooling%20....pdf) in TPAMI 2015.
1. [Batch renormalization](http://papers.nips.cc/paper/6790-batch-renormalization-towards-reducing-minibatch-dependence-in-batch-normalized-models.pdf) from NIPS 2017.

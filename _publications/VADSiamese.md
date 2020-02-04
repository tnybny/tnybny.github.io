
---
title: "Learning a distance function with a siamese network to localize anomalies in videos"
collection: publications
permalink: /publication/VADSiamese
excerpt: 'This paper presents a new metric learning approach to localize anomalies in surveillance video.'
date: 2020-01-31
venue: 'WACV 2020'
paperurl: 'https://arxiv.org/abs/2001.09189'
---

[[Paper link]](https://arxiv.org/abs/2001.09189)

## Abstract

This work introduces a new approach to localize anomalies in surveillance video. The main novelty is the idea of using a Siamese convolutional neural network (CNN) to learn a distance function between a pair of video patches (spatio-temporal regions of video). The learned distance function, which is not specific to the target video, is used to measure the distance between each video patch in the testing video and the video patches found in normal training video. If a testing video patch is not similar to any normal video patch then it must be anomalous. We compare our approach to previously published algorithms using 4 evaluation measures and 3 challenging target benchmark datasets. Experiments show that our approach either surpasses or performs comparably to current state-of-the-art methods.


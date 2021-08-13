---
title: "Perceptual metric learning for video anomaly detection"
collection: publications
permalink: /publication/g-VADSiamese
excerpt: 'This paper generalizes a previous metric learning approach to operate with arbitrary-sized region proposals to localize anomalies in surveillance video'
date: 2021-01-31
venue: 'MVA 2021'
paperurl: 'https://www.merl.com/publications/docs/TR2021-028.pdf'
---

[[Paper link]](https://www.merl.com/publications/docs/TR2021-028.pdf)

## Abstract

This work introduces a new approach to localize anomalies in surveillance video. The main
novelty is the idea of using a Siamese convolutional neural network (CNN) to learn a metric
between a pair of video patches (spatio-temporal regions of video). The learned metric, which
is not specific to the target video, is used to measure the perceptual distance between each
video patch in the testing video and the video patches found in normal training video. If a
testing video patch is far from all normal video patches then it must be anomalous. We further
generalize the approach from operating on video patches from a fixed grid to arbitrary-sized
region proposals. We compare our approaches to previously published algorithms using 4
evaluation measures and 3 challenging target benchmark datasets. Experiments show that
our approaches either surpass or perform comparably to current state-of-the-art methods
whilst enjoying other favorable properties.

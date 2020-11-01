---
title: "Multimodal Deep Learning Based Crop Classification Using Multispectral and Multitemporal Satellite Imagery"
collection: publications
permalink: /publication/Multi modal crop clf
excerpt: 'This paper presents a multimodal strategy for crop classification using multispectral imagery and NDVI phenology time series'
date: 2020-08-01
venue: 'KDD 2020'
paperurl: 'https://dl.acm.org/doi/abs/10.1145/3394486.3403375'
---

[[Paper link]](https://dl.acm.org/doi/abs/10.1145/3394486.3403375)

## Abstract

The Food and Agriculture Organization (FAO) of the United Nations predicts that in order to meet the needs of the expected 3 billion population growth by 2050, food production has to increase by 60%. Therefore, monitoring and mapping crops accurately is essential for estimating food production during each crop growing season across the globe. Traditionally, multispectral remote sensing imagery has been widely used for mapping crops worldwide. However, single date imagery does not capture temporal characteristics (phenology) of growing crops, leading to imprecise crop maps and food estimates. On the other hand, purely temporal classification approaches also produce inaccurate crop maps as they do not account for spatial autocorrelations. In this paper, we present a multimodal deep learning solution that jointly exploits spatial-spectral and phenological properties to identify major crop types. Using a two stream architecture, spatial characteristics are captured via a spatial stream consisting of very high resolution images (single date, 1m, 3-spectral bands, USDA NAIP) with a CNN and the phenological characteristics via a temporal stream images (biweekly, 250m, MODIS NDVI) with an LSTM. Experimental results show that the proposed multimodal solution reduces prediction error by 60%.

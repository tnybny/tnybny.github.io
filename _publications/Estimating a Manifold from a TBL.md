---
title: "Estimating a Manifold from a Tangent Bundle Learner"
collection: publications
permalink: /publication/manifold-estimation-from-TBL
excerpt: 'This paper is about estimating a manifold from a tangent bundle learner.'
date: 2019
venue: 'arXiv'
paperurl: 'https://arxiv.org/abs/1906.07661'
---
Manifold hypotheses are typically used for tasks such as dimensionality reduction, interpolation, or improving classification performance. In the less common problem of manifold estimation, the task is to characterize the geometric structure of the manifold in the original ambient space from a sample. We focus on the role that tangent bundle learners (TBL) can play in estimating the underlying manifold from which data is assumed to be sampled. Since the unbounded tangent spaces natively represent a poor manifold estimate, the problem reduces to one of estimating regions in the tangent space where it acts as a relatively faithful linear approximator to the surface of the manifold. Local PCA methods, such as the Mixtures of Probabilistic Principal Component Analyzers method of Tipping and Bishop produce a subset of the tangent bundle of the manifold along with an assignment function that assigns points in the training data used by the TBL to elements of the estimated tangent bundle. We formulate three methods that use the data assigned to each tangent space to estimate the underlying bounded subspaces for which the tangent space is a faithful estimate of the manifold and offer thoughts on how this perspective is theoretically grounded in the manifold assumption. We seek to explore the conceptual and technical challenges that arise in trying to utilize simple TBL methods to arrive at reliable estimates of the underlying manifold.
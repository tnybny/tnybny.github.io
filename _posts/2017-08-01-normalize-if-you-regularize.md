---
title: 'Normalize if you regularize'
date: 2017-08-01
permalink: /posts/2018/08/normalize-if-you-regularize/
tags:
  - z-score normalization
  - L1/L2 regularization
---

There is a world of preprocessing methods from which a scientist has to choose. In each of the preprocessing tasks of cleaning, missing data handling, standardizing, encoding, binning, binarizing and etcetera, there are further choices to make. Some of these choices are data dependent, some not. Some are model dependent, some not. I want to talk about one such choice: z-score normalizing your training set before training.

For many models such as logistic regression, the theory behind the model itself provides no reason to normalize your training data. For the longest time, I avoided doing it when presented with the choice as I did not have any evidence to support doing it. The rationale behind this was that when you have so many choices as a scientist, you should always have a reason to do anything. However, I recently realized that I overlooked one subtle interaction, that between normalizing and regularization.

There is evidence to support **normalization helps when you are also using regularization** and here it is - 
L1/L2 regularization aim to penalize the magnitude of your regression coefficients. If your features are in different units and by consequence different scales, then those of natively higher magnitude are biased to having larger coefficients and are better candidates for L1/L2 regularization, even though they might be the most discriminative features. Normalization puts all the features in the same scale, effectively controlling for this effect before deciding how to apply the regularization.

Of course, this does depend on the classifier and regularizer you use. For example, random forests generalize by ensembling, not L1 or L2, so this would not apply; neural networks are free to learn features at their own scale, so again this wouldn't apply. In some cases there are other reasons to normalize, such as to make gradient flow easier with neural nets.

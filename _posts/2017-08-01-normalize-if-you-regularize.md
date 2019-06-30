---
title: 'Normalize if you regularize'
date: 2017-08-01
permalink: /posts/2018/08/normalize-if-you-regularize/
tags:
  - z-score normalization
  - L1/L2 regularization
---

There is a world of preprocessing methods from which a data scientist has to choose. In each of the preprocessing tasks of cleaning, missing data handling, standardizing, encoding, binning, binarizing and etcetera, there are further choices to make. Some of these choices are data dependent, some not. Some are model dependent, some not. I want to talk about one such choice: z-score normalizing your training set before training.

For man models such as logistic regression, the theory behind the model itself provides no reason to normalize your training data. And as all good data scientists should do, I avoided doing it when presented with the choice as I did not have any evidence to support doing it. Others would have done it as a precautionary measure stating the reason that "it surely cannot hurt". I maintain that this is bad practice. When you have so many choices as a data scientist, you should always have a reason to do anything. But that aside, I realized that I overlooked one subtle interaction, that between normalizing and regularization.

There is evidence to support **normalization helps when you are also using regularization** and here it is - 
L1/L2 regularization aim to penalize the magnitude of your regression coefficients. If your different features are in different units, then those that have more variance are biased to having larger coefficients and are better candidates for L1/L2 regularization, even though they might be the best (most discriminative) features.

One caveat: This does depend on the classifier and regularizer you use. Random forests generalize by ensembling, not L1 or L2, so this does not apply to RFs.

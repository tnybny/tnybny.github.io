---
title: 'On balancing classes for an imbalanced class problem'
date: 2017-09-01
permalink: /posts/2017/09/On-balancing-classes/
tags:
  - imbalanced classes
---

The common suggestion that balancing classes in an imbalanced class problem boosts accuracy, either through oversampling the minority class or undersampling the majority class, is an over-generalization.
In many cases, this is simply not true unless the minority class oversampling process includes data augmentation. Intuitively, this is because the amount of information in your minority class is fixed even if you oversample it (you're just creating duplicates, which do not change the decision boundary). I realize this discussion is restricted to discriminative modeling.

## Experiment: 
Starting with ~70/30 imbalanced training set, I divided the set randomly into 70/30 training and validation split. Then I either left the training set as is or balanced it by undersampling the majority class. I built logistic regression models on unbalanced and balanced datasets and performed post-thresholding to test if I had the optimal threshold for prediction.
The table below shows the summarized results of validation set accuracy as a function of type of balancing and post-threshold. The model built on the balanced dataset did no better than the unbalanced dataset.

Dataset\threshold | 0.5 | Best
--- | --- | ---
Unbalanced | 73% | 73% 
Balanced\* | 56%	| 73% 

\* by undersampling the majority class

Clearly, the **best accuracy is achieved at a threshold of 0.5 for the unbalanced training set**. This is to be expected form the theory of logistic regression. Post-thresholding cannot achieve a better result.
Moreover, the **coefficient matrices of both models were the very similar, but they had different intercept vectors**. The conclusion is that the decision boundary has not changed by balancing of classes.

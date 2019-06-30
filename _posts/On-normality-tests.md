---
title: 'On normality tests'
date: 2017-01-01
permalink: /posts/2017/01/On-normality-tests/
tags:
  - Test for normality
  - Statistical tests
---

I recently came across this very interesting problem. I wanted to verify if some of my data could be assumed to be normally distributed since I wanted to use statistical methods that assumed the same. As I have always read, I assumed that I would just run the Shapiro-Wilk test or the Anderson Darling test on my data and if the null hypothesis is not rejected, I would go ahead with the normality assumption. 

Just to be doubly careful, I searched and stumbled upon [this blog post](https://www.r-bloggers.com/normality-tests-don%E2%80%99t-do-what-you-think-they-do/). What the author says is that these normality tests are
1. Dependent on sample size
2. Are null hypothesis tests against the assumption of normality
As a result, for small sample sizes even a big departure from normality isn't detected and for large sample sizes even the smallest departure is!

Conclusion: A Q-Q plot is required in addition to these tests for verification.

Keep in mind though that 
> 1. You can never, no matter how much data you collect, conclusively determine that it was generated from an exactly normal > distribution. 
> 2. Your data is not generated from an exactly normal distribution (no real data is).

- Ian Fellows
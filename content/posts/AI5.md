---
title: "Machine Learning Research Papers, Takeaways, and Directions"
date: 2024-01-24T16:50:26+12:00
draft: false
tags: ["machine learning", "support if stuck"]
categories: ["tech"]
---

This collection of resources delves into various challenges encountered during the development and optimization of machine learning models. Each section focuses on a specific issue commonly faced in practical applications and presents approaches to mitigate these challenges.

<!--more-->

### Loss Function Converging to Multiple Local Minima

[On Large-Batch Training For Deep Learning: Generalization Gap And Sharp Minima](https://arxiv.org/pdf/1609.04836.pdf)

Imagine facing a situation where the loss function converges to different stable values during multiple runs with identical parameters. It is most likely that the loss function is very curvy and has multiple local minima where the training is getting stuck.

To improve the training process, reduce the batch size and decrease the learning rate, as they respectively help the model overcome local minima and prevent overshooting the global minimum of the loss function.

### Low Sensitivity TPR

[Class-imbalanced classifiers for high-dimensional data](https://academic.oup.com/bib/article/14/1/13/304457?login=true)

The true positive rate (TPR, also called sensitivity) is calculated as TP/TP+FN. TPR is the probability that an actual positive will test positive. 

Imagine dealing with a logistic regression spam detection model that has high overall accuracy (99%) but fails to detect 90% of spam emails.

To improve the model's ability to detect more than 10% of spam emails, decrease the class probability threshold. This adjustment increases the model's sensitivity, marking more cases as the positive class (spam), thereby improving the likelihood of spam detection, although it may lower precision. This is covered in the Discussion section of the paper at this [link](https://academic.oup.com/bib/article/14/1/13/304457?login=true).

### Limited Examples of Positive Cases

[SMOTE: Synthetic Minority Over-sampling Technique](https://www.jair.org/index.php/jair/article/view/10302)

When dealing with a limited amount of spam email data, the method most likely to detect the greatest number of valid spam emails is oversampling using SMOTE. This technique involves adding synthetic data points to the minority class, helping address the imbalance in the dataset and providing more information for the model to learn from.

### Missing Feature Values

[A Comparison of Six Methods for Missing Data Imputation](https://www.omicsonline.org/open-access/a-comparison-of-six-methods-for-missing-data-imputation-2155-6180-1000224.php?aid=54590)

In a scenario with highly imbalanced target label classes and multiple feature columns contain missing values. The proportion of missing values across the entire data frame is less than 5%.

To minimize bias due to missing values is, use supervised learning to predict missing values based on other features is suggested. Different supervised learning approaches might have different performances, but any properly implemented supervised learning approach should provide the same or better approximation than mean or median approximation, hence supervise learning is the preferred solution. 

#### Reading List
- [Handling Missing Values when Applying Classification Models](https://jmlr.csail.mit.edu/papers/volume8/saar-tsechansky07a/saar-tsechansky07a.pdf)
- [What Do We Do with Missing Data? Some Options for Analysis of Incomplete Data](https://www.annualreviews.org/doi/10.1146/annurev.publhealth.25.102802.124410)
- [Amazon Feature Processing](https://docs.aws.amazon.com/machine-learning/latest/dg/feature-processing.html)
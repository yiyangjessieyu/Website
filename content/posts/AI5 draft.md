---
title: "Machine Learning Research Papers, Takeaways, and Directions"
date: 2024-01-30T10:49:26+12:00
draft: false
tags: ["machine learning"]
categories: ["tech"]
---

### [On Large-Batch Training For Deep Learning: Generalization Gap And Sharp Minima](https://arxiv.org/pdf/1609.04836.pdf)

Imagine facing a situation where the loss function converges to different stable values during multiple runs with identical parameters. It is most likely that the loss function is very curvy and has multiple local minima where the training is getting stuck.

To improve the training process, reduce the batch size and decrease the learning rate, as they respectively help the model overcome local minima and prevent overshooting the global minimum of the loss function.

### [Class-imbalanced classifiers for high-dimensional data](https://academic.oup.com/bib/article/14/1/13/304457?login=true)

Imagine dealing with a logistic regression spam detection model that has high overall accuracy (99%) but fails to detect 90% of spam emails.

To improve the model's ability to detect more than 10% of spam emails, decrease the class probability threshold. This adjustment increases the model's sensitivity, marking more cases as the positive class (spam), thereby improving the likelihood of spam detection, although it may lower precision. This is covered in the Discussion section of the paper at this [link](https://academic.oup.com/bib/article/14/1/13/304457?login=true).

### [SMOTE: Synthetic Minority Over-sampling Technique](https://www.jair.org/index.php/jair/article/view/10302)

When dealing with a limited amount of spam email data, the method most likely to detect the greatest number of valid spam emails is oversampling using SMOTE. This technique involves adding synthetic data points to the minority class, helping address the imbalance in the dataset and providing more information for the model to learn from.

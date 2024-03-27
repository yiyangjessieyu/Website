---
title: "March '24 News"
date: 2024-03-13T16:01:26+12:00
draft: true
tags: ["ai"]
categories: ["tech"]
---
News from March 2024 that caught my attention.

<!--more-->

## [The State of Competitive Machine Learning](https://mlcontests.com/state-of-competitive-machine-learning-2023/)

### Computer Vision:
- Unlike in NLP, leading computer vision models still largely hadn’t converged on a single architecture.
- Things looked similar throughout 2023: both CNNs (convolutional neural networks) and Transformers were used for vision, and most competition winners still used CNN-based architectures.
- This lack of architectural convergence is backed up by research — a [2023 paper compared NFNets (a CNN-based architecture) against Vision Transformers](https://arxiv.org/abs/2310.16764?ref=mlcontests), and found that “NFNets match the reported performance of Vision Transformers with comparable compute budgets.”
- The winner of DrivenData’s Tick Tick Bloom competition, where participants used satellite imagery to detect specific types of bacteria in bodies of water, showed that deep learning isn’t necessarily the right tool for all computer vision problems. Their solution used a combination of k-nearest-neighbours and a LightGBM model, with features including climate data and the colour of the water. They noted “I tried using a CNN model with satellite images. Unfortunately, this type of model resulted in very high RMSEs. After some analysis, I suspect that the quality and resolution of the satellite images, as well as the accuracy of the positions, made it very difficult to fit the CNN model well.”
- Popular Working Toolkits:

![alt text](image-6.png)
---
title: "Stanford CS229: Machine Learning Course, Lecture 1"
date: 2023-09-03T15:31:26+12:00
draft: false
tags: ["course", "machine learning"]
categories: ["tech"]
---

Thank you [Andrew Ng](https://www.andrewng.org/) for the [lecture](https://www.youtube.com/watch?v=jGwO_UgTS7I).

Resources:
- [Program info](https://learn.stanford.edu/Social-AI-YouTube.html?utm_source=YouTube&utm_medium=Social&utm_campaign=cs229_lec1_2018),
- [Syllabus](http://cs229.stanford.edu/syllabus-autumn2018.html),
- [Enrol online](https://www.coursera.org/specializations/machine-learning-introduction?action=enroll).


## Notes

An intro to machine learning and statistical pattern recognition. Talked about both supervised and unsupervised learning as well as learning theory, reinforcement learning and control. Explored recent applications of machine learning and design and develop algorithms for machines.

Example at [45.50](https://youtu.be/jGwO_UgTS7I?t=2750) was a nice way to illustrate dimensionality, explain how higher multi-dimensional problems become difficult to graph, and hence introduce the motivation behind Support Vector Machines (SVM) - which help overcome this challenge. 

First time seeing how autonomous driving vechnical work behind the scenes at [52:54](https://youtu.be/jGwO_UgTS7I?t=3174) - how the model is matching what it is seeing with the car's front camera with the steering choices made by the human, and eventually learn to make those matches itself. So given video footage, able to learn what steering choice to make. 

All CS229 Lecture Notes [here](https://github.com/yiyangjessieyu/Machine-Learning/blob/main/lectures/main_notes.pdf)

### Definitions

Supervised learning: Learning to map an input x to an appropriate output y. Eg. Learning to map a video footage of the road in front of the car with the appropriate driving choices. 

Regression: Continuous.

Classification: Categorical. 
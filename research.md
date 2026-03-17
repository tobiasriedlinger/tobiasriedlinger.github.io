---
layout: default
title: Research
description: 
---

{% include nav.html %}

My research generally lies at the intersection of mathematics and machine learning.

## Reliable AI and Uncertainty Quantification 
Neural networks are great.
It is uncomfortable to admit, but they do some things better than I.
But they are also bad at knowing when they don't know something.
This research direction addresses this shortcoming by developing methods to quantify the uncertainty of model predictions and safety mechanisms.

## Statistical Deep Learning
So far from my point of view the most convincing and sensible notion of successful learning: **P**robably **A**pproximately **C**orrect learning captures that training data is drawn from a probability distribution covering worst case scenarios.
Proving PAC learnability for deep learning models involves a variety of mathematical tools and requires understanding their interplay and connections.

## Data Curation and Active Learning
I was looking through failure cases of a deep object detection model in order to understand why its performance was worse than we expected.
When I saw that some of the ground truth annotations were missing, I felt bad for my model and swore to avenge it.
This research direction deals with systematic methods for discovering annotation errors in large-scale datasets injected by human labelers.
As a related discipline, I investigate how to smartly use annotation budgets in the context of active learning.
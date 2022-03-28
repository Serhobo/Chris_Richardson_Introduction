---
title: Welcome back, I got you Flowers. I am over 98% certain.
subtitle: Please see the below link to my second contribution to a Kaggle Compettion. I was able to achieve a higher accurracy from our tutorial code by creating a train / dev / test system, and trialing different hyperparamets. Take a look for yourself!

# Summary for listings and search engines
summary: Please see the below link to my second contribution to a Kaggle Compettion. I was able to achieve a higher accurracy from our tutorial code by creating a train / dev / test system, and trialing different hyperparamets. Take a look for yourself!

# Link this post with a project
projects: [School Project]

# Date published
date: "2022-3-25T19:54:00Z"

# Date updated
lastmod: "2022-3-25T19:54:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: true

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Kaggle Datasets**](https://storage.googleapis.com/kaggle-datasets-images/8782/12270/c3af536d14e386a2bfd356d1cd84b67e/dataset-cover.jpg?t=2018-01-06-14-10-54)'
  focal_point: ""
  placement: 2
  preview_only: false

authors:
- admin

tags:
- Academic
- NN
- ML

categories:
- School Project
- Personal Favorite
---

## Overview

https://github.com/Serhobo/Image-Identifier


## Overview of the Project

The basic premise of this project was to create an image classifer that could accurately classify 5 different types of flowers from a supplied database. We are given code by a **PyTorch** tutorial called **Training a Classifier**. Using the majority of this code as a building block, I created an image classifier that could accurately pick out the 5 types of flowers at approximately **98.4%**. In decreasing order of significance of the reference in my code, I used the code from the Pytorch tutorial, another neural network program, and the pytorch documentation as references. 

## Process and Results

I tested out the effects of numerous changes to my own code. Over adjusting the hyperparameters, playing with batch sizing, playing with various resizes of images, increases epoch, and generating additional test images using transformations all had various levels of benefits.

## PRETTY SLIDES AND GRAPHS AND STUFF
# Featured image
# Place an image named `featured5.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**3 Universities**](https://www.frontiersin.org/articles/10.3389/fpls.2021.618028/full)'
  focal_point: ""
  placement: 2
  preview_only: false

## Contributions

 I will not be able to fully adding and swapping out the variables originally used within the creation of the decision trees. Additionally, I tested various random states, as well as number of estimators and depth of decision trees. I found that swapping out SibSp for Embarked, and noticed a flat increase of over 4% on its accuracy. Due to the incompleteness of several of the variables included in the training data, the inclusion of some attributes were limited due to the nature of the competition and my shortcomings in my knowledge. Both of these are appropriates areas of improvement.

The original accuracy of my default transformation of all the photos was roughly . With my contributions, it was improved to 0.77751. This equated to a 4.78% increase in effectiveness.

## Sources

Data and Code for the Kaggle competition was provided by [Kaggle](https://www.kaggle.com/c/titanic) itself.
Website created using website templates released under the [MIT](https://github.com/wowchemy/wowchemy-hugo-modules/blob/master/LICENSE.md) license.

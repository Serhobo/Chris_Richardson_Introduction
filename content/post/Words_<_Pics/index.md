---
title: Hello again, I got News for you, or I might have Healthy Living for you?
subtitle: My first attempt at a text identifier has left me questioning my own word identification. I was able to refine my model by incorporating some changes I have not yet seen implemented by any other!

# Summary for listings and search engines
summary: My first attempt at a text identifier has left me questioning my own word identification. I was able to refine my model by incorporating some changes I have not yet seen implemented by any other!

# Link this post with a project
projects: [School Project]

# Date published
date: "2022-4-17T21:28:39Z"

# Date updated
lastmod: "2022-4-17T21:28:39Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: true

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**Confuse with your Own "News"**](https://www.jonathancresswell.co.uk/breakingnews/fb.jpg)'
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

https://github.com/Serhobo/NewsMaker


## Overview of the Project

This project surrounds the idea of idenitifying articles based on their headlines. This requires an in-depth dive into hte requirements for Naive Bayes Classifer. My first idea on improving the field of classifers I haved come across is to include the brief description with the title into a new column.

## Process and Results

My first improvement was to include the short descirption into a combined column with the headline. This allowed for addition words that could be attached to the news categories. This led to the below results:

## Results as of 4/17/2022:

Train Accuracy : 65.70%

Dev Accuracy  : 57.33%

## Process

This process was less involved than the picture classifier. This is largely due to the concept sinking in with me less than the image one. The image program allowed for an easy visualization of the progress of analysizing the model. This text model is less intuitive, and therefore harder to program to.

## Contributions

I combined the description and headline into one column to create additional data for the training model. I also renoved any hyperlink structuring and any non-alphabet chracter. Thie cleaned up text allowed me more information to train the model to.

## Sources

Data for the Kaggle database was provided by [Rishabh Misra](https://www.kaggle.com/datasets/rmisra/news-category-dataset).

Help on how to properly implement plotter. [Hamza Manssor](https://www.kaggle.com/code/hamzamanssor/news-category-classification).

Pytorch documentation. [Pytorch](https://pytorch.org/vision/stable/auto_examples/plot_transforms.html#sphx-glr-auto-examples-plot-transforms-py).

Website created using website templates released under the [MIT](https://github.com/wowchemy/wowchemy-hugo-modules/blob/master/LICENSE.md) license.

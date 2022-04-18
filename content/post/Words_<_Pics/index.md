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

UPDATE

I tested out the effects of numerous changes to my own code. Over adjusting the hyperparameters, playing with batch sizing, playing with various resizes of images, increases epoch, and generating additional test images using transformations all had various levels of benefits. I will not be able to fully demonstrate the effectiveness some of these had as this assignment was an extensive learning experience. If I were to repeat this assignment with my new knowledge, I would not follow my following procedure again. This is purely a reflection of the process I took.

UPDATE

## Results as of 4/17/2022:

Train Accuracy : 65.70%

Dev Accuracy  : 57.33%

## Process

UPDATE

After following the tutorial's coding process, my first step and first contribution to a reference was to change the input to the trainloader and testloader to the new Flower databser. I did not anticipate the level of difficulty this would present for the first time. After battling with a series of error codes, I looked through a few tutorials. I landed upon one in particular that satisified my code's error reports.

At this point, I believed I was getting great results in interesting progress in my program. What I did not realize was that all of my test results until Friday, March 25th, 2022, were flawed. I was testing my network to images it may or may not have already seen. My initial choice to increase the training of the network, was to show it all images. This is fundamentally flawed and lead to infalted success at first. I implemented a new training/testing suggestion from my March 25th lecture with Professor Park. I separated out the images prior to any training into 3 separate datasets, train / dev / test. My results **TANKED** instantly. I was seeing accuracies as high as 99.5% prior to this, and was astonished at the ease I was experiencing. This new method pulled the wool from my eyes, and ignited a curiousity to refine this program properly. 

My first set as a novice, was to over-tune the parameters to squeak out a few percentage point improvements for the entire Flower dataset. This was not only timeconsuming, but ultimately pointless. Each model, that was trained, would experience a different randomized training set. This meant that fine-tuning the parameters was probability based, and non repeatable improvment. 

This lead me to trialing different ranges of epochs for running the training data through my model. I ran 5 varying tests of epoch magnitudes, prior to grasphing how to utlize the autographing functions available to me. My original results lead me to believe that anything after epoch = 30, would no longer provide a sufficent improvement. To cement this idea, I ran an epoch of 1000 that lasted roughly 15 hours. After seeing the results the next afternoon, I realized everything I previously "learned" about my choice for an epoch was practically worthless. The only real information I learned was that every set of parameters. images, etc. has different Loss results and therefore diffrenet optimal epoch.

UPDATE

## Contributions

UPDATE

The original accuracy of my default transformation of all the photos was roughly 53%. This transformation was based off of copied code from the Pytorch tutorial and observations from Georgii Sirotenko's program. My contribution to both of these references was making them vaiably work together, as they conflicted originally. 

I was unaware of the ability to concat datasets included within Torch. I was made aware of this option through Georgii Sirotenko's program. This is a straight forward process, so my contributions were limited. I achieved incorporating all of my own datasets into this potion of code.

While this is what all good programmers should do, I read the documentation for image manipulation within Pytorch. I selected all of my image transformations from this list in the library's documentation.

UPDATE

## Sources

Data for the Kaggle database was provided by [Rishabh Misra](https://www.kaggle.com/datasets/rmisra/news-category-dataset).

Help on how to properly implement plotter. [Hamza Manssor](https://www.kaggle.com/code/hamzamanssor/news-category-classification).

Pytorch documentation. [Pytorch](https://pytorch.org/vision/stable/auto_examples/plot_transforms.html#sphx-glr-auto-examples-plot-transforms-py).

Website created using website templates released under the [MIT](https://github.com/wowchemy/wowchemy-hugo-modules/blob/master/LICENSE.md) license.

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

I tested out the effects of numerous changes to my own code. Over adjusting the hyperparameters, playing with batch sizing, playing with various resizes of images, increases epoch, and generating additional test images using transformations all had various levels of benefits. I will not be able to fully demonstrate the effectiveness some of these had as this assignment was an extensive learning experience. If I were to repeat this assignment with my new knowledge, I would not follow my following procedure again. This is purely a reflection of the process I took.

## Results as of 3/24/2022:

Accuracy of the network on the 864 dev images: 85 %

Dev Accuracy for class: daisy is 80.8 %

Dev Accuracy for class: dandelion is 86.9 %

Dev Accuracy for class: rose  is 87.9 %

Dev Accuracy for class: sunflower is 89.2 %

Dev Accuracy for class: tulip is 84.2 %

Accuracy of the network on the 1080 test images: 53 %

Test Accuracy for class: daisy is 40.0 %

Test Accuracy for class: dandelion is 61.6 %

Test Accuracy for class: rose  is 48.9 %

Test Accuracy for class: sunflower is 53.5 %

Test Accuracy for class: tulip is 57.7 %

## Results as of 3/27/2022:

Accuracy of the network on the 864 dev images: 98 %

Dev Accuracy for class: daisy is 98.7 %

Dev Accuracy for class: dandelion is 99.5 %

Dev Accuracy for class: rose  is 98.8 %

Dev Accuracy for class: sunflower is 98.6 %

Dev Accuracy for class: tulip is 98.5 %

Accuracy of the network on the 1080 test images: 97 %

Test Accuracy for class: daisy is 97.1 %

Test Accuracy for class: dandelion is 99.3 %

Test Accuracy for class: rose  is 96.6 %

Test Accuracy for class: sunflower is 95.1 %

Test Accuracy for class: tulip is 96.2 %

## Process

After following the tutorial's coding process, my first step and first contribution to a reference was to change the input to the trainloader and testloader to the new Flower databser. I did not anticipate the level of difficulty this would present for the first time. After battling with a series of error codes, I looked through a few tutorials. I landed upon one in particular that satisified my code's error reports.

At this point, I believed I was getting great results in interesting progress in my program. What I did not realize was that all of my test results until Friday, March 25th, 2022, were flawed. I was testing my network to images it may or may not have already seen. My initial choice to increase the training of the network, was to show it all images. This is fundamentally flawed and lead to infalted success at first. I implemented a new training/testing suggestion from my March 25th lecture with Professor Park. I separated out the images prior to any training into 3 separate datasets, train / dev / test. My results **TANKED** instantly. I was seeing accuracies as high as 99.5% prior to this, and was astonished at the ease I was experiencing. This new method pulled the wool from my eyes, and ignited a curiousity to refine this program properly. 

My first set as a novice, was to over-tune the parameters to squeak out a few percentage point improvements for the entire Flower dataset. This was not only timeconsuming, but ultimately pointless. Each model, that was trained, would experience a different randomized training set. This meant that fine-tuning the parameters was probability based, and non repeatable improvment. 

This lead me to trialing different ranges of epochs for running the training data through my model. I ran 5 varying tests of epoch magnitudes, prior to grasphing how to utlize the autographing functions available to me. My original results lead me to believe that anything after epoch = 30, would no longer provide a sufficent improvement. To cement this idea, I ran an epoch of 1000 that lasted roughly 15 hours. After seeing the results the next afternoon, I realized everything I previously "learned" about my choice for an epoch was practically worthless. The only real information I learned was that every set of parameters. images, etc. has different Loss results and therefore diffrenet optimal epoch.

## Contributions

The original accuracy of my default transformation of all the photos was roughly 53%. This transformation was based off of copied code from the Pytorch tutorial and observations from Georgii Sirotenko's program. My contribution to both of these references was making them vaiably work together, as they conflicted originally. 

I was unaware of the ability to concat datasets included within Torch. I was made aware of this option through Georgii Sirotenko's program. This is a straight forward process, so my contributions were limited. I achieved incorporating all of my own datasets into this potion of code.

While this is what all good programmers should do, I read the documentation for image manipulation within Pytorch. I selected all of my image transformations from this list in the library's documentation.

## Sources

Data for the Kaggle database was provided by [Alexander Mamaev](https://www.kaggle.com/datasets/alxmamaev/flowers-recognition).

Code for the NN was provided by [Pytorch](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html#sphx-glr-beginner-blitz-cifar10-tutorial-py).

Help loading images and understanding transformations. [Georgii Sirotenko](https://www.kaggle.com/code/georgiisirotenko/pytorch-flowers-translearing-ensemble-test-99-67).

Pytorch documentation. [Pytorch](https://pytorch.org/vision/stable/auto_examples/plot_transforms.html#sphx-glr-auto-examples-plot-transforms-py).

Website created using website templates released under the [MIT](https://github.com/wowchemy/wowchemy-hugo-modules/blob/master/LICENSE.md) license.

---
title: Do I take the Blue Berry or the Red Berry?(Later parts of report being updated 5/2/22)
subtitle: Unlike a popular movie series, I don't want to see how deep "the rabbithole" goes. I assume other people feel like me, especially when identifying plants on a hike, or camping trip. I attempt to tackle identifying common edible and harmful plants. Take a look for yourself!

# Summary for listings and search engines
summary: Unlike a popular movie series, I don't want to see how deep "the rabbithole" goes. I assume other people feel like me, especially when identifying plants on a hike, or camping trip. I attempt to tackle identifying common edible and harmful plants. Take a look for yourself!

# Link this post with a project
projects: [School Project]

# Date published
date: "2022-4-29T19:54:00Z"

# Date updated
lastmod: "2022-4-29T19:54:00Z"

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: true

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: 'Image credit: [**The Scariest Things**](https://scariesthings.com/2019/04/26/happy-arbor-day-fifteen-killer-plant-movies-you-know-they-have-it-in-for-us-right/)'
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

https://github.com/Serhobo/Edible-or-Harmful/


## Overview of the Project

The idea for this task came about after a converstation I had with a coworker.  In a passing comment, he complained about why didn't one already exist. My last image classifer had only 5 image classes, so expanding it to 86 species of plants provided a wide range of complications. The first issue and toughest one, personally, was finding out my last image classifer's testing data was tainted and inflated my results. Transformed versions of the test images were included in my training dataset. I started this program based off my previous image classifer, so old sources are still relevant, as well as contributions to them.

## Process and Results

The first step in my process was to clean up legacy code and markdowns with knowledge I did not posess at the time of that project. Examples of this include, but not limited to, deleting sections of commented out code, markdowns with erroneous data, and shortening lines of code. With the basic housekeeping completed, I quickly located where I dragged in the testing images on accident. However, with the way the dataset was constructed in the previous challenge, I was not aware of a way to properly prevent this. However, with the next step of the project, I could correct this issue by building my dataset in the structure I desired.

  I combined three separate datasets I found on Kaggle. They are as follows: Wild Edible Plants (https://www.kaggle.com/datasets/ryanpartridge01/wild-edible-plants), Edible Wild Plants (https://www.kaggle.com/datasets/gverzea/edible-wild-plants) and Poisonous Plants Images (https://www.kaggle.com/datasets/nitron/poisonous-plants-images). I combined all of these into one larger set of images, verified that the testing images were not resused in the training or validation, and loaded it at https://www.kaggle.com/datasets/richardsonchris/edible-or-harmful-plant-dataset.

## Results as of 4/29/2022 (only non-transformed training images):

  #Accuracy of the network on the 496 test images: 8 %
  
  -Test Accuracy for class: Alfalfa is 20.0 %
  -Test Accuracy for class: Allium is 0.0 %
  -Test Accuracy for class: Asparagus is 0.0 %
  -Test Accuracy for class: Blue Vervain is 0.0 %
  -Test Accuracy for class: Borage is 0.0 %
  -Test Accuracy for class: Broadleaf Plantain is 0.0 %
  -Test Accuracy for class: Bull Thistle is 0.0 %
  -Test Accuracy for class: Burdock is 0.0 %
  -Test Accuracy for class: Calendula is 40.0 %
  -Test Accuracy for class: castor_oil_plant is 40.0 %
  -Test Accuracy for class: Cattail is 60.0 %
  -Test Accuracy for class: Chickweed is 60.0 %
  -Test Accuracy for class: Chicory is 0.0 %
  -Test Accuracy for class: Chive Blossom is 0.0 %
  -Test Accuracy for class: Cleavers is 0.0 %
  -Test Accuracy for class: Coltsfoot is 0.0 %
  -Test Accuracy for class: Common Mallow is 0.0 %
  -Test Accuracy for class: Common Milkweed is 0.0 %
  -Test Accuracy for class: Common Sow Thistle is 0.0 %
  -Test Accuracy for class: Common Vetch is 40.0 %
  -Test Accuracy for class: Common Yarrow is 20.0 %
  -Test Accuracy for class: Coneflower is 20.0 %
  -Test Accuracy for class: Cow Parsley is 0.0 %
  -Test Accuracy for class: Cowslip is 0.0 %
  -Test Accuracy for class: Creeping Charlie is 40.0 %
  -Test Accuracy for class: Crimson Clover is 20.0 %
  -Test Accuracy for class: Crithmum Maritimum is 0.0 %
  -Test Accuracy for class: Curly Dock is 60.0 %
  -Test Accuracy for class: Daisy Fleabane is 80.0 %
  -Test Accuracy for class: Dandellion is 0.0 %
  -Test Accuracy for class: dieffenbachia is 0.0 %
  -Test Accuracy for class: Downy Yellow Violet is 0.0 %
  -Test Accuracy for class: Elderberry is 0.0 %
  -Test Accuracy for class: Evening Primrose is 0.0 %
  -Test Accuracy for class: Fennel is 0.0 %
  -Test Accuracy for class: Fern Leaf Yarrow is 0.0 %
  -Test Accuracy for class: Field Pennycress is 0.0 %
  -Test Accuracy for class: Fireweed is 60.0 %
  -Test Accuracy for class: Forget Me Not is 60.0 %
  -Test Accuracy for class: foxglove is 0.0 %
  -Test Accuracy for class: Gardenia is 0.0 %
  -Test Accuracy for class: Garlic Mustard is 0.0 %
  -Test Accuracy for class: Geranium is 0.0 %
  -Test Accuracy for class: Ground Ivy is 0.0 %
  -Test Accuracy for class: Harebell is 0.0 %
  -Test Accuracy for class: Henbit is 0.0 %
  -Test Accuracy for class: Herb Robert is 40.0 %
  -Test Accuracy for class: Japanese Knotweed is 0.0 %
  -Test Accuracy for class: Joe Pye Weed is 0.0 %
  -Test Accuracy for class: Knapweed is 0.0 %
  -Test Accuracy for class: Kudzu is 0.0 %
  -Test Accuracy for class: Lambs Quarters is 40.0 %
  -Test Accuracy for class: lilies is 0.0 %
  -Test Accuracy for class: lily_of_the_valley is 20.0 %
  -Test Accuracy for class: Mallow is 0.0 %
  -Test Accuracy for class: Mayapple is 0.0 %
  -Test Accuracy for class: Meadowsweet is 0.0 %
  -Test Accuracy for class: Milk Thistle is 0.0 %
  -Test Accuracy for class: Mullein is 0.0 %
  -Test Accuracy for class: New England Aster is 0.0 %
  -Test Accuracy for class: oleander is 0.0 %
  -Test Accuracy for class: Partridgeberry is 0.0 %
  -Test Accuracy for class: Peppergrass is 0.0 %
  -Test Accuracy for class: Pickerelweed is 20.0 %
  -Test Accuracy for class: Pineapple Weed is 0.0 %
  -Test Accuracy for class: Prickly Pear Cactus is 0.0 %
  -Test Accuracy for class: Purple Deadnettle is 0.0 %
  -Test Accuracy for class: Queen Annes Lace is 60.0 %
  -Test Accuracy for class: Ramsons is 0.0 %
  -Test Accuracy for class: Red Clover is 0.0 %
  -Test Accuracy for class: rhubarb is 0.0 %
  -Test Accuracy for class: Sheep Sorrel is 0.0 %
  -Test Accuracy for class: Shepherds Purse is 0.0 %
  -Test Accuracy for class: Spring Beauty is 0.0 %
  -Test Accuracy for class: Sunflower is 20.0 %
  -Test Accuracy for class: Supplejack Vine is 0.0 %
  -Test Accuracy for class: Tea Plant is 0.0 %
  -Test Accuracy for class: Teasel is 0.0 %
  -Test Accuracy for class: Toothwort is 0.0 %
  -Test Accuracy for class: Vervian Mallow is 0.0 %
  -Test Accuracy for class: Wild Bee Balm is 0.0 %
  -Test Accuracy for class: Wild Black Cherry is 0.0 %
  -Test Accuracy for class: Wild Grape Vine is 0.0 %
  -Test Accuracy for class: Wild Leek is 0.0 %
  -Test Accuracy for class: wisteria is 0.0 %
  -Test Accuracy for class: Wood Sorrel is 0.0 %

While these resutls are not much at this point, I am certain I have corrected the issue of a tainted testing data. One thing I noticed was that in the training data for asparagus was several pictures of store bought ones or canned ones. Therefore, I removed it from the database for all subsequent trails.

## Results as of 5/1/2022:

  #Accuracy of the network on the 491 test images: 31.00 %
  
  -Test Accuracy for class: Alfalfa is 40.00 %
  -Test Accuracy for class: Allium is 20.00 %
  -Test Accuracy for class: Blue Vervain is 20.00 %
  -Test Accuracy for class: Borage is 40.00 %
  -Test Accuracy for class: Broadleaf Plantain is 20.00 %
  -Test Accuracy for class: Bull Thistle is 0.00 %
  -Test Accuracy for class: Burdock is 80.00 %
  -Test Accuracy for class: Calendula is 60.00 %
  -Test Accuracy for class: castor_oil_plant is 100.00 %
  -Test Accuracy for class: Cattail is 20.00 %
  -Test Accuracy for class: Chickweed is 60.00 %
  -Test Accuracy for class: Chicory is 0.00 %
  -Test Accuracy for class: Chive Blossom is 0.00 %
  -Test Accuracy for class: Cleavers is 60.00 %
  -Test Accuracy for class: Coltsfoot is 60.00 %
  -Test Accuracy for class: Common Mallow is 80.00 %
  -Test Accuracy for class: Common Milkweed is 0.00 %
  -Test Accuracy for class: Common Sow Thistle is 80.00 %
  -Test Accuracy for class: Common Vetch is 20.00 %
  -Test Accuracy for class: Common Yarrow is 80.00 %
  -Test Accuracy for class: Coneflower is 20.00 %
  -Test Accuracy for class: Cowslip is 0.00 %
  -Test Accuracy for class: Creeping Charlie is 80.00 %
  -Test Accuracy for class: Crimson Clover is 40.00 %
  -Test Accuracy for class: Crithmum Maritimum is 20.00 %
  -Test Accuracy for class: Curly Dock is 80.00 %
  -Test Accuracy for class: Daisy Fleabane is 80.00 %
  -Test Accuracy for class: Dandellion is 20.00 %
  -Test Accuracy for class: dieffenbachia is 20.00 %
  -Test Accuracy for class: Downy Yellow Violet is 0.00 %
  -Test Accuracy for class: Elderberry is 100.00 %
  -Test Accuracy for class: Evening Primrose is 60.00 %
  -Test Accuracy for class: Fennel is 0.00 %
  -Test Accuracy for class: Fern Leaf Yarrow is 60.00 %
  -Test Accuracy for class: Field Pennycress is 40.00 %
  -Test Accuracy for class: Fireweed is 100.00 %
  -Test Accuracy for class: Forget Me Not is 20.00 %
  -Test Accuracy for class: foxglove is 100.00 %
  -Test Accuracy for class: Gardenia is 100.00 %
  -Test Accuracy for class: Garlic Mustard is 40.00 %
  -Test Accuracy for class: Geranium is 100.00 %
  -Test Accuracy for class: Ground Ivy is 0.00 %
  -Test Accuracy for class: Harebell is 40.00 %
  -Test Accuracy for class: Henbit is 20.00 %
  -Test Accuracy for class: Herb Robert is 60.00 %
  -Test Accuracy for class: Japanese Knotweed is 0.00 %
  -Test Accuracy for class: Joe Pye Weed is 20.00 %
  -Test Accuracy for class: Knapweed is 0.00 %
  -Test Accuracy for class: Kudzu is 60.00 %
  -Test Accuracy for class: Lambs Quarters is 40.00 %
  -Test Accuracy for class: lilies is 0.00 %
  -Test Accuracy for class: lily_of_the_valley is 40.00 %
  -Test Accuracy for class: Mallow is 20.00 %
  -Test Accuracy for class: Mayapple is 40.00 %
  -Test Accuracy for class: Meadowsweet is 20.00 %
  -Test Accuracy for class: Milk Thistle is 60.00 %
  -Test Accuracy for class: Mullein is 0.00 %
  -Test Accuracy for class: New England Aster is 0.00 %
  -Test Accuracy for class: oleander is 0.00 %
  -Test Accuracy for class: Partridgeberry is 0.00 %
  -Test Accuracy for class: Peppergrass is 60.00 %
  -Test Accuracy for class: Pickerelweed is 60.00 %
  -Test Accuracy for class: Pineapple Weed is 20.00 %
  -Test Accuracy for class: Prickly Pear Cactus is 20.00 %
  -Test Accuracy for class: Purple Deadnettle is 40.00 %
  -Test Accuracy for class: Queen Annes Lace is 80.00 %
  -Test Accuracy for class: Ramsons is 20.00 %
  -Test Accuracy for class: Red Clover is 20.00 %
  -Test Accuracy for class: rhubarb is 0.00 %
  -Test Accuracy for class: Sheep Sorrel is 0.00 %
  -Test Accuracy for class: Shepherds Purse is 0.00 %
  -Test Accuracy for class: Spring Beauty is 20.00 %
  -Test Accuracy for class: Sunflower is 40.00 %
  -Test Accuracy for class: Supplejack Vine is 20.00 %
  -Test Accuracy for class: Tea Plant is 0.00 %
  -Test Accuracy for class: Teasel is 0.00 %
  -Test Accuracy for class: Toothwort is 28.57 %
  -Test Accuracy for class: Vervian Mallow is 15.38 %
  -Test Accuracy for class: Wild Bee Balm is 8.33 %
  -Test Accuracy for class: Wild Black Cherry is 0.00 %
  -Test Accuracy for class: Wild Grape Vine is 15.38 %
  -Test Accuracy for class: Wild Leek is 21.43 %
  -Test Accuracy for class: wisteria is 23.08 %
  -Test Accuracy for class: Wood Sorrel is 15.38 %


## Future Considerations

Due to the importance of nailing done the model prior to adding the additional functionalities, the stretch goal of adding a video feed to identify the plant has been placed on hold. 

## Contributions

The original code comes from the Pytorch tutorial and observations from various pytorch documentations. My contribution from this original code is substanstial. I have implemented it to an entirely new dataset, creates test, validation, and train folders, and changed all of the parameters. A warning handler was copied from a stack overflow question as it is only 2 lines and directly addresses my problem.

I combined three different databases into one larger one to expand the use of this model. The three databases can be found below.

While this is what all good programmers should do, I read the documentation for image manipulation within Pytorch. I selected all of my image transformations from this list in the library's documentation.

## Sources

Code for the NN was provided by [Pytorch](https://pytorch.org/tutorials/beginner/blitz/cifar10_tutorial.html#sphx-glr-beginner-blitz-cifar10-tutorial-py).

Warning handlger from StackOverflow by [Mike](https://stackoverflow.com/questions/14463277/how-to-disable-python-warnings).

Pytorch documentation. [Pytorch](https://pytorch.org/vision/stable/auto_examples/plot_transforms.html#sphx-glr-auto-examples-plot-transforms-py).

First Database [Wild Edible Plants](https://www.kaggle.com/datasets/ryanpartridge01/wild-edible-plants)
Second Database [Edible Wild Plants](https://www.kaggle.com/datasets/gverzea/edible-wild-plants)
Third Database [Poisonous Plant Images](https://www.kaggle.com/datasets/nitron/poisonous-plants-images)

Website created using website templates released under the [MIT](https://github.com/wowchemy/wowchemy-hugo-modules/blob/master/LICENSE.md) license.

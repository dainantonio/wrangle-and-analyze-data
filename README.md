# Wrangle and Analyzedata

# Table of Contents

1. Project Overview
    i. [Introduction](#introduction)
    ii. [What Software do I need](#what softwares do I need?)
2. [The Data](#the data)
3. [Key Points](#key points)
4. [Conclusion](#conclusion)
5. [References](#references)

## Introduction<a class="anchor" id="introduction"></a>
   
Real-world data rarely comes clean. Using Python and its libraries, I gathered data from a variety of sources and in a variety of formats, assessed its quality and tidiness, then cleaned it. 

The dataset that I wrangled was the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. 

These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.

## What Software do I Need?<a class="anchor" id="what softwares do I need"></a>
 
I worked on my local machine with Jupyter Notebook. You can use whatever you are comfortable with like VS Code etc.

## The following packages (libraries) need to be installed. You can install these packages via conda or pip. 

* Pandas

* NumPy

* Requests

* Tweepy

* json

## Installation links for softwares:

* Git for windows - for terminal application using Git Bash

* Python using Anaconda (latest version for windows)

* Visual Studio Code Editor (for windows)

I used Google Docs to document my project in PDF format, you can use whatever text editor you like.

My goal was to wrangle this Twitter data in order to create interesting and trustworthy analyses and visualizations. However, we had to gather more data to get the best analysis and visualizations.

The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced." Of the 5000+ tweets, I have filtered for tweets with ratings only (there are 2356).

# The Data<a class="anchor" id="the data"></a>
 
## Enhanced Twitter Archive

The WeRateDogs Twitter archive contains basic tweet data for all 5000+ of their tweets, but not everything. One column the archive does contain though: each tweet's text, which I used to extract rating, dog name, and dog "stage" (i.e. doggo, floofer, pupper, and puppo) to make this Twitter archive "enhanced."

## Additional Data via the Twitter API

Back to the basic-ness of Twitter archives: retweet count and favorite count are two of the notable column omissions. Fortunately, this additional data can be gathered by anyone from Twitter's API. Well, "anyone" who has access to data for the 3000 most recent tweets, at least. But we, because we have the WeRateDogs Twitter archive and specifically the tweet IDs within it, can gather this data for all 5000+. And guess what? We're going to query Twitter's API to gather this valuable data.

## Image Predictions File

One more cool thing: I ran every image in the WeRateDogs Twitter archive through a neural network that can classify breeds of dogs. The results: a table full of image predictions (the top three only) alongside each tweet ID, image URL, and the image number that corresponded to the most confident prediction (numbered 1 to 4 since tweets can have up to four images).

## Key Points<a class="anchor" id="key points"></a>
   
Key points to keep in mind when data wrangling for this project:
* We only want original ratings (no retweets) that have images. Though there are 5000+ tweets in the dataset, not all are dog ratings and some are retweets.

* Fully assessing and cleaning the entire dataset requires exceptional effort so only a subset of its issues (eight (8) quality issues and two (2) tidiness issues at minimum) need to be assessed and cleaned.

* Cleaning includes merging individual pieces of data according to the rules of tidy data.

* The fact that the rating numerators are greater than the denominators does not need to be cleaned. This unique rating system is a big part of the popularity of WeRateDogs.

* We do not need to gather the tweets beyond August 1st, 2017. We can, but note that we won't be able to gather the image predictions for these tweets since we don't have access to the algorithm used.

## Project Details<a class="anchor" id="project details"></a>
  
We will perform the following tasks in this project:

* Data wrangling, which consists of:

* Gathering data

* Assessing data

* Cleaning data

Storing, analyzing, and visualizing our wrangled data

Reporting on 1) data wrangling efforts and 2) data analyses and visualizations

## Conclusion<a class="anchor" id="conclusion"></a>
   

## References<a class="anchor" id="references"></a>
  

# Wrangle and Analyzedata

Real-world data rarely comes clean. Using Python and its libraries, I gathered data from a variety of sources and in a variety of formats, assessed its quality and tidiness, then cleaned it. 

The dataset that I wrangled was the tweet archive of Twitter user @dog_rates, also known as WeRateDogs. WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. 

These ratings almost always have a denominator of 10. The numerators, though? Almost always greater than 10. 11/10, 12/10, 13/10, etc. Why? Because "they're good dogs Brent." WeRateDogs has over 4 million followers and has received international media coverage. This archive contains basic tweet data (tweet ID, timestamp, text, etc.) for all 5000+ of their tweets as they stood on August 1, 2017.

## What Software Do I Need?
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

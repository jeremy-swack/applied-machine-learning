# Project 4: Final Project Plan 

[Back to Home Page](https://jeremy-swack.github.io/applied-machine-learning/)

## Problem Statement:

As said by Chinese investor Connie Chan, “TikTok is the first mainstream consumer app where artificial intelligence IS the product.” Anyone who has used the social media platform can attest to this; the main feature of the app is the incredibly powerful recommendation engine known as the “For You Page.” TikTok learns a user’s interests using a variety of different data to allow the app to almost always recommend a video that the user will enjoy. This has led to TikTok having one of the longest retention times of any app, beating out social media titans like Facebook and Instagram. 

Although TikTok has not released the specifics of their algorithm, many have theorized how it works. For TikTok to recommend a video to users, it needs to know who to push it out to. It is likely that TikTok uses a variety of machine learning techniques to extract as much information as possible from a video. For this project, I want to try and replicate these techniques to find what makes a TikTok go viral.

## The Inputs:

* Videos scraped using the unofficial TikTok API 
  * Can use the the get_trending() function to gather approximately 2000 TikToks in one scrape
  * Will collect data over multiple days
  * Want to collect at least 2000-10000 videos
* Individual video metadata
  * Video ID
  * Caption
  * Sound
  * Number of followers the creator has
  * If it's an Ad
* Natural Language Processing Component
  * Audio is converted to text using a speech recognition package
* Computer Vision 
  * Using the YOLOv3 model, roughly 80 different objects can be identified
      
## The Model:

* Still unclear what the model will be, but likely an ANN because it will be able to predict non-linear relationships which I believe will be likely
* Model will output number of likes for the video
* Can make visualizations to show what the most common words in captions were of viral TikToks, most common objects, etc.

## Donald Trump Twitter Analysis


## Overview

The central focus of this project is to analyze Donald Trump's Twitter activity using different methods of text mining. We also use several approaches to determine the influence Donald Trump's rhetoric has had on the popularity and the messaging of hate groups within the U.S. We focus on Trump's Twitter activity to investigate any similarities between his Twitter feed and those of various domestic hate groups or individual extremists. We think that Trump's rhetoric has changed vastly over the last decade. Considering his shift in tone, we are interested in exploring the evolution of hate speech during this time period. 

Based on this, our main research question is: Is Trump's Twitter activity associated with the Twitter activity of hate groups? 
We predict that since the beginning of Trump's presidential campaign, and continuing into his presidency, the Twitter activity of hate groups has increased and may even reflect Trump's Twitter activity. 

We begin with several text analyses of Trump's tweets using methods such as n_grams and word correlations. We then use methods, such as topic modeling, to compare his Tweets to domestic hate groups.

## Use

We use the package tidytext (Silge and Robinson 2016) and other relevant text analysis tools in R to analyze the Twitter data that we downloaded. First, we start by evaluating word correlations using N-Grams. We then use Network Analysis to map most commonly correlated words. We also use NRC Lexicon in our sentiment analysis to classify the tweets as "positive" or "negative". Finally, we use approaches in Topic Modeling to find natural group of topic associated across all of our Twitter data. We present various visualizations to highlight the trends of the Twitter activity of Trump and hate groups. 


## Data Used

We obtained data from the [Trump Twitter Archive](http://www.trumptwitterarchive.com/). This source compiled Trump's Twitter activity into a dataset that includes information on the date he tweeted, the text he tweeted, and retweet counts. We use Trump's tweets from 2009 to present day.

We also used the [Southern Poverty Law Center](https://www.splcenter.org/fighting-hate/extremist-files/individual) to gather a list of individuals who have been identified as extremist. They range from being white Nationalist to anti-Islamic or anti-Semitic. We identified their twitter handles, or their affiliated organization's twitter handles, and scraped their most recent tweets. Unfortunately, Twitter API allows us to go back to tweets six to nine days in the past, so we collected whatever tweets were available to us from May 5^th^ 2017, to as early as April 26^th^, 2017.

The final data set, for Trumps tweets, has approximately 30,866 observations, and the hate group data set comprises of a total of 75 individuals and groups and 62,252 observations.


## Progress Log

April 15th : 

  - Collected list of extremists from the Southern Poverty Law Center website (https://www.splcenter.org/fighting-hate/extremist-files/individual).
  - Collected twitter handles of the extremists or affiliated organization from twitter.

April 18th : 

  - Using R, we coded a loop to extract the most recent tweets (maximum 1500) from each extremist and Trump's twitter feed.
  - These were appended to form one final data set.
          
April 21st:

  - Began cleaning and formatting Twitter data. We used the tidy text format to create dataset with one-token-per-row, with each row as as 
a single word. 
  
April 28th: 

  -Used N-Grams and Word correlations to visualize Trump's Twitter activity. 

April 30th:
  
  -Conducted Sentiment Analysis using NRC lexicon to evaluate the emotional content of Trump's tweets. 

May 4th: 

  -Conducted analysis comparing Trump's tweets using Term Frequency and Topic Modeling. 

May 6th: 

  -Made final adjustments to code and finished write-up of the R markdown file. 
  -Compiled code and write-up in a html file. Created [website](https://drb88.github.io/data_science/).


## Credits

Contributors:

  - Ryan Buckner
  - Mariam Ghavalyan 
  - Chinmaya Holla
  - Raiyan Kabir


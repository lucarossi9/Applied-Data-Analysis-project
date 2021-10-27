# ADA-2021-project-fix-it

## Title : Finding an author's position based on clustering techniques

## Abstract

 From an intuitive standpoint it’s often considered that common beliefs and values can lead to similar opinions perspectives, therefore we tend to hypothesize that given a shared background and beliefs people would often write and think in a related way.
 
In statistics one can speak about this similarity as correlation, if for two similar authors we know that there is a correlation between the positions they have regarding a certain topic, then by looking at quotes from the first author we can make an educated guess about the positions of the second author, given the statistical significance of said correlation.  

An interesting question one can make is if it's possible to predict the position of a certain author related to a certain topic even without quotes from him about this specific topic. The goal of our project is to solve this problem, namely by using **clustering** and **sentimental analysis** we try to predict an author's position even without meaningful quotes on the topic.

## Research Questions

Some research questions that we would like to address in this project:
* Are there topics where authors usually have the same set of positions, for example is a pro euthanasia author more likely to be pro abortion?
* Can we predict a person's political party from their position on a set of topics?

## Proposed Dataset

No external dataset will be used, therefore only the Quotebank dataset wil be used.

## Methods

* Filter quotes by topic:
  - For each topic define a set of words intimately related to the topic
  - Filter the dataset in search of quotes that mention at least one of the words related to the topic
 
* Access the position of the authors to a certain topic:
  - Develop Sentiment Analysis techniques using LSTMs (in our case we will be using TextBlob), then use the aforementioned techniques to attribute a value (between -1 and 1) to each quote.
  - Average each author's quotes sentiment value, then use the mean to compute whether the author is a pro or against the topic.

* Predict author's position based on clustering techniques:
  - Using a variant of K-nearest neighbors predict the author's position
  - Compute the accuracy of the prediction defined above

* Statistical Analysis:
  - Compute the correlation between the positions on each set of topics
  - Compute the null hypotheses and see the statistical significance of deviations. 
  - ...
  
## Proposed timeline

* 25th October - 31st October:
  -

* 1st November - 7th November:
  -

* 8th November - 12th November:
  -


## Organization within the team

to be determined

## Questions for TAs

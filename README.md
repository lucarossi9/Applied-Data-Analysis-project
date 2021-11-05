# ADA-2021-project-fix-it

## Title : Finding an author's position based on clustering techniques

## Abstract

In the 21st century public opinion is crucial for political figures to understand how their base feels about them, thus studying the media approval rating can be of utmost importance. 

Media approval rating can take many forms, traditionally one would think in a classification scheme where we could label people support of a certain public figure as pro, against or neutral, however a different representation could be labelling using a continuous value. Indeed by using a continuous value we can see with more clarity if people's opinion are more polarized or not, for example for elections it's very important to be able to distinguish between let's say a bimodal distribution and a bell curve shaped distribution, since in the first case the probability of getting undecided voters to vote for you it's smaller than in the other case.

Our focus will be on showing the evolution of the polarization of popularity for different political figures, as well as a careful analysis of what this meant in term of political events. 

## Research Questions


## Proposed Dataset

The Quotebank dataset wil be used jointly with Special attributes dataset.

## Methods

* Filter quotes by person:
  - For each person define a set of aliases
  - Filter the dataset in search of quotes that mention at least one of the aliases
 
* Map the people's opinion on this person:
  - Develop Sentiment Analysis techniques using LSTMs (in our case we will be using TextBlob), then use the aforementioned techniques to attribute a value (between -1 and 1) to each quote.
  
* Analysis of media approval rating:
  - Compute the distribution and polarization metrics for each (person, timestamp)
  - Relate it to important event in the political career of said person
  - Compute a statistical test to see if two samples came from the same distributions (before and after a important political event)
 

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

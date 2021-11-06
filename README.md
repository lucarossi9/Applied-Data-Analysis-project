# ADA-2021-project-fix-it

## Title : Discovering popularity of famous american politicians 

## Abstract

In the 21st century media coverage is a crucial factor for political figures. By studying the number of times a certain politician is quoted in media outlets (in our case New York Times), we can have a rough measure of how much interest does the media address to this politician.
In our analysis we will study the evolution of the number of citations of some of the most important american politicians over the last few years and we will compare their evolution to the most important events in their carreer in order to see if there is any causation or correlation. We will then add some more analysis distinguishing the speakers (who quoted a certain politician) by religion, nationality and political party in order to have a better and fragmented view of the causal effects. In the end we will compare our work with Google Trends data in order to see if the conventional media outlets caption the online interest well.

## Research Questions



## Proposed Dataset

The Quotebank dataset will be used jointly with Special attributes dataset, additionally Google trends data will be used for producing meaningful comparisons.

## Methods

* Filter quotes by person:
  - For each politician we look for his surname in each quote in the dataset.
  - Refilter again the result removing all the quotes whose author is the politician himself.
 
* Analysis of the result
  - Provide the time series of the occurrences for different politicians over different periods of time trying to analyse which are the events in the life of a politician which cause the politician to be quoted more.
  - Tell the story of the american political scene from a mediatic point of view, comparing the evolution of the distribution of the main american politicians over the years 2015-2020.
  - Compare our results with Google Trends data in order to see if there is any match between the number of quotes linked to a certain politician and how much is he/she searched on google. We expect the two distribution to be similar but not the same since some scandal/events can have different a impact on different types of media (the user base of Google is quite different from the reader base of New York Times and the content shared online is inherently different from the conventional news). 
  - Merge the QuoteBank dataset with the special attribute dataset in order to understand important information on the people who quoted a given politician. We intend to analyse how the timeseries distribution of occurences of a given politician in a quote changes within different age groups, religion groups and political parties.

* Sensitivity analysis
  - Standardize features such as age, categorize other features such as political party, religion, ethnic group. Label each author to have either mentioned a certain political figure or not.
  - Use the aforementioned features to compute a logistic regression model to predict if the author mentioned a certain political figure or not, essentially computing the propensity scores.
  - Match pairs of persons with the same propensity score in order to create meaningful treated and control groups.
  - Explicitely compare the distributions of both treated and control groups, in the end compute odds ratio.

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

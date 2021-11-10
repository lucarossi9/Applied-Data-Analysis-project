# ADA-2021-project-fix-it

## Title : An analysis of the american political scene from a mediatic point of view 

## Abstract

In the 21st century, media coverage is crucial for political figures.
By studying the number of quotes on a given politician and on a given date, we can have a rough measure of how much interest the medias addressed to the politician that day. In our analysis we will study the evolution of the number of citations on some of the most important American politicians over the last few years and we will compare it to important events in their career telling in this way the story of the American political scene from a mediatic point of view. We will then analyse the causation/correlation between such events and the number of citations also divinding the speakers (the author of quotes on a given politician) by age/sex/nationality to have a better understanding of the causal effects. Finally, we will compare our work with Google Trends to see if the conventional media outlets capture the online interest well.

## Research Questions

- Who are the people whose quotes refer more to a given politician ?

- Is there any correlation between the number of quotes from conventional media that mention a certain politician and the number of online views?

- Are their characteristics such as age, political party or religion indicative of the number of quotes this person has on a certain political figure?

- Which events in the life of a politician can be associated to an increase of the number of quotes referred to him ? 

- Are political elections or pre-elections debates a period in which the number of quotes on a given politician is rising ?

- How 2016 political elections contributed to an increase or decrease of the number of quotes referred to Trump and Clinton ?

- Which is the period in which we assisted to the maximum number of quotes on a politician (Trump for example) and why ?

- Which events in the life of a politician can be associated to an increase of the number of quotes referred to him over different groups (for example dividing the speakers by age, nationalities, political parties,...)

## Proposed Dataset

The Quotebank (quotes centric version) dataset will be used jointly with Special attributes dataset, additionally Google trends data will be used for producing meaningful comparisons and Quotebank (article centric version) will be used to find the date for each quote.

## Methods

##### 1. Filter quotes by person:
  * For each politician we look for his surname in each quote in the dataset and we create a dataframe containing just these rows.
  * For each politician we remove from the previously created dataframe the rows in which it is the politician himself speaking and the rows in which the name of people with the same surname of the politician appear. In this way we can remove from the previously created dataframe all the quotes pronounced by the politician himself and the rows not speaking about the politician but speaking about other people with the same surname.
  
##### 2. Replace the ids in the speaker attributes file
* We replace the ids in the speaker attributes file to have a meaningful dataframe containing all the informations about the speaker, we will use it later for the analysis part.

##### 3. Extract the dates from the Quotebank file
* For each filtered quote, we extract from the quotebank (article centric dataset) the dates of all the articles containing that quote and we add them to the filtered dataframe created in point 1).

##### 4. Analysis of the result
  - Provide the time series (number of quotes related to a given politicians vs time) for different politicians and for different periods of time.
  - We will analyse which are the events in the life of a politician which cause the politician to appear more on quotes.
  - Tell the story of the American political scene from a mediatic point of view, comparing the evolution of the time series for the main American politicians over the years 2015-2020.
  - Compare our results with Google Trends data in order to see if there is any match between the number of quotes linked to a certain politician and how much is he/she searched on google over different periods. We expect the two distribution to be similar but not the same since some scandal/events can have a different impact on different types of media (the user base of Google is quite different from the reader base of New York Times and the content shared online is inherently different from the conventional news). 
  - Merge the previously created dataframe with the speaker attribute dataframe in order to understand important information on the people who quoted a given politician. We intend to analyse how the time series distribution of occurrences of a given politician changes within different age groups, religion groups and political parties. From this analysis we can understand which events are the one which increase the most the number of quotes on a given politician for each group of people.

##### 5. Correlation and hypothesis testing analysis
 - We will try to understand the features of the speakers (present in the speaker attribute file) which are the most correlated with a huge number of quotes on a given politician. 
 - We will do chi squared hypothesis test in order to understand if a given features is independent on the number of quotes on a certain politician.

## Proposed timeline

* 25th October - 31st October:
  - Decide the idea of the project

* 1st November - 7th November:
  - Check the feasibility (checking if sentimental analysis is working)--> Some ideas were discarded

* 8th November - 12th November:
  - Preparing the data as described and show the feasibility of the idea

## Organization within the team



## Questions for TAs

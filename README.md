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

### 1. Filter quotes by person:
  * For each politician we look for his surname in each quote in the dataset and we create a dataframe containing just these rows.
  * For each politician we remove from the previously created dataframe the rows in which it is the politician himself speaking and the rows in which the name of people with the same surname of the politician appear. In this way we can remove from the previously created dataframe all the quotes pronounced by the politician himself and the rows not speaking about the politician but speaking about other people with the same surname.
  
2. Replace the ids in the speaker attributes file to have a meaningful dataframe containing all the informations about the speakers.

3. For each filtered quote, extract from the quotebank (article centric dataset) the dates of all the articles containing that quote and we add them to the filtered dataset in point 1)


4. Analysis of the result
  - Provide the time series of the occurrences for different politicians over different periods of time trying to analyse which are the events in the life of a politician which cause the politician to appear more on quotes.
  - Tell the story of the american political scene from a mediatic point of view, comparing the evolution of the distribution of the main american politicians over the years 2015-2020.
  - Compare our results with Google Trends data in order to see if there is any match between the number of quotes linked to a certain politician and how much is he/she searched on google. We expect the two distribution to be similar but not the same since some scandal/events can have a different impact on different types of media (the user base of Google is quite different from the reader base of New York Times and the content shared online is inherently different from the conventional news). 
  - Merge the QuoteBank dataset with the special attribute dataset in order to understand important information on the people who quoted a given politician. We intend to analyse how the timeseries distribution of occurences of a given politician in a quote changes within different age groups, religion groups and political parties.

5. Sensitivity analysis
  - Our initial hypothesis could be that people aged more than 40 tend to speak more about a certain politician with respect to people aged less than 40. We will validate or discredit this belief using sensitivity analysis.
  - Standardize features such as age, categorize other features such as political party, religion, ethnic group. Label each author to have either mentioned a certain political figure or not.
  - Use the aforementioned features to compute a logistic regression model to predict if the author mentioned a certain political figure or not, essentially computing the propensity scores with our observed covariates such as gender, age, nationality,religion, ...
  - Match pairs of persons with the same propensity score in order to create meaningful treated and control groups (with the same dimension of samples) , split this pairs based on the value of the age (above or below 40).
  - Explicitely compare the distributions of both treated and control groups, in the end compute odds ratio to validate or discredit our initial hypothesis.

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

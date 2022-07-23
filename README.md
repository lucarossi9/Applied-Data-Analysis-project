# Applied Data Analysis 2021-project

# An analysis of the american political scene from a mediatic point of view 

## Abstract

In the 21st century, media coverage is crucial for political figures.
By studying the number of quotes referred to a given politician on a given date, we can have a rough measure of how much interest the media addressed to the politician that day. Using Quotebank Dataset, we studied the evolution of the number of citations of two of the most famous American politicians (Donald Trump and Hillary Clinton) over the last few years, and we compared it to key events in their careers to present the story of the American political scene of the years 2015-2017 from a mediatic point of view. Moreover, we compared our work with Google Trends to see if the conventional media outlets capture online interest well. Finally, using t-tests, confidence intervals, and an interpretable machine learning model (linear/logistic regression), we understood which features of the authors of the quotes could predict whether the latter will speak about Clinton or Trump.

To have a look at the datasory : https://diogosoares22.github.io/ada-fix-it/

To have a look at the repository of the story: https://github.com/diogosoares22/ada-fix-it
## Research Questions

- Who between Trump and Clinton has more quotes in different periods from 2015 to 2017 and why ?

- Which events in the life of a politician can be associated to an increase of the number of quotes referred to him ? 

- Are political elections or pre-elections debates a period in which the number of quotes on a given politician is rising ?

- Is there any statistically significant difference between the age and the ratios men/women of Trump/Clinton speakers ?

- Are nationalities of the speakers different from Clinton and Trump speakers ? If yes can we understand why ?

- Which of the speaker attributes are the most relevant to make the speaker having quotes referred to Trump or to Clinton ?

## Proposed Dataset

The Quotebank (quotes centric version) dataset will be used jointly with Special attributes dataset, additionally Google trends data will be used for producing meaningful comparisons and Quotebank (article centric version) will be used to find the date for each quote.

## Methods

### Data preparation 

##### 1. Filter quotes by person:
 * For each politician we look for his surname in each quote in the dataset and we create a dataframe containing just these rows.
 * For each politician we remove from the previously created dataframe the rows in which it is the politician himself speaking and the rows in which the name of people with the same surname of the politician appears. In this way we can remove from the previously created dataframe all the quotes pronounced by the politician himself and the rows not speaking about the politician but speaking about other people with the same surname.
  
##### 2. Replace the ids in the speaker attributes file
* We merge the quotes with the speaker attribute file so that we also have all the relevant information about the speakers.

##### 3. Extract the dates from the Quotebank file
* For each filtered quote, we extract from the quotebank (article centric dataset) the dates of all the articles containing that quote and we add them to the filtered dataframe created in point 1).

##### 4. Google Trends
* We download the data from Google Trends related to the queries referred to Trump or Clinton in the years 2015-2017.

### Results

##### 5. Timeseries
* Provide the time series (number of quotes related to a given politicians vs time) for Trump and Clinton and for the years 2015-2017.
* We analyse which are the events in the life of a politician which cause the politician to have more quotes referred to him/her.
* Tell the story of the American political scene from a mediatic point of view for the years 2015-2017.
* Compare our results with Google Trends data in order to see if there is any match between the number of quotes linked to a certain politician and how much is he/she searched on google over different periods ---> some matches were found but also some mismatches, we explained why.

##### 6. Speaker attributes analysis
* Use t-test to find statistically significant difference in mean of the age of the Trump's speakers and Clinton speaker's ---> Clinton speakers are older.
* Use confidence intervals to understand if there is a statistically significant ratio #men/#women between the Trump's and Clinton's speakers. ---> The ratio is bigger for Trump's speakers.
* Look at the difference in the distribution of the nationality, we noticed some differences and some similarity, we explained why this happens.
* We build a machine learning model to explain which of the attributes of the speakers are the most relevant for them to have quotes referred to Trump or to Clinton.

## Proposed timeline

##### Milestone 2

* 25th October - 31st October:
  - Decide the idea of the project

* 1st November - 7th November:
  - Check the feasibility (checking if sentimental analysis is working)--> Some ideas were discarded

* 8th November - 12th November:
  - Preparing the data as described and show the feasibility of the idea

##### Milestone 3
 * First week: Started writing the code (mainly time series part)
 
 * Second week: Finish the codes (differences between speaker attributes of the two groups and machine learning model)
 
 * Third week: Data Story

## Organization within the team

##### Milestone 2

- Luca : Filtering data
- Diogo : Merge files
- Goncalo : Plotting and veryfing feasibility

##### Milestone 3

- Luca : Wrote all the codes for milestone 3, wrote timeseries part of the datastory, wrote google trend comparison part of datastory, wrote machine learning part of the datastory (mainly the tree part), fixing code quality, reviewing the datastory
- Diogo : Review the code, wrote machine learning model part and age analysis part of the datastory
- Goncalo : Wrote the part of the nationality of the datastory

### See Code Organization.md to understand how we have organized the notebooks

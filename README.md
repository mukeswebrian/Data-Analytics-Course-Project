# Data-Analytics-Course-Project

For the project, you are provided with a dataset to analyze using the skills learned in the course.

When working on the project, you are encouraged to consider the different stages of the data life cycle
and the importance of using the right tools to efficiently answer as many of the project questions as you can. 

Feel free to be creative in how you present your findings to answer each project question. At the very minimum,
you are expected to create a dashboard in Tableau Public (https://public.tableau.com/en-us/s/) with at least 3 different visualizations to help answer 
some of the project questions.


## Dataset description:
The dataset contains the daily number of webpage visits for several Wikipedia webpages. 
(if you are not familiar with Wikipedia, you can check it out here https://en.wikipedia.org/wiki/Main_Page).
The dataset includes daily page visit counts for 1,500 Wikipedia pages starting on 2016-01-01 until 2016-12-31.

Dataset source: Kaggle.com

# Data Life Cycle - Guided Exercises:

## Plan
1. Assume that you are working for the Wikipedia company as a data analyst, what are some potentially valuable business insights that can be obtained from the provided Wikipedia dataset?
2. What challenges do you anticipate will arise when trying to analyse the dataset provided? For each challenge, outline a potential solution for overcoming the challenge.
3. What are some risks or limitations of relying on the dataset provided to inform decisions about the Wikipedia platform?

## Collect
1. Imagine you had a chance to talk to the team responsible for collecting the dataset provided, what are some key questions you would ask them about how the data was collected in order to gain a better understanding of the underlying assumptions in the data?
2. The data file provided is a single extract (batch) for a 1 year period. Now imagine you needed to track the top trending topics based on page visits on a daily basis, what might be a better way of accessing the data besides an Excel file?
3. A colleague has proposed that you should store the provided data into a SQL database so that you can run queries on it. What are some challenges you anticipate to encounter? How might you overcome these challenges?

## Process
1. In the current dataset, each row represents a unique page and the number of visits the page received for each day of the year. Write a Python script to transform the data such that it has only three columns ie. page_name, date, and number of visits.  
In the transformed dataset, each page will have multiple row entries, each corresponding to a different day of the year.
2. Compare the transformed dataset to the original one provided, which one is easier to analyze? Why?
3. Modify your script such that the transformed dataset contains the following additional columns: page_language, access_device_type, day_of_the_week, month

## Analyze
1. Comment on the distribution of daily page visits based on the dataset provided. Are there outliers? You are encouraged to use data visualizations to answer this question.
2. For each of the criteria below, identify 2 pages that meet the criterion, and create a time series plot of the pages' visits throughout the year.
    - Criterion 1: Relatively steady number of visits throughout the year.
    - Criterion 2: Significantly higher number of visits later in the year compared to earlier in the year.
    - Criterion 3: Significantly lower number of visits later in the year compared to earlier in the year.
3. Identify some page pairs that have a high correlation in the number of visits. Use a scatter plot and/or a time series plot to illustrate these correlations.

## Share
1. Create a dashboard that allows a user to easily visualize the following:
    - The top 20 pages based on number of visits.
    - The user should be able to filter and view the top pages for any day of the year.
    - The user should also able to filter the list based on the page.
    - The user should also be able to filter the list based on the device type used to visit the page.
    
2. Create a dashboard that allows a user to easily visualize a time series plot of the visits for an arbitrary page.


## Project Questions:
1. what were some of the most trending search topics on Wikipedia on the following days? Using the provided dataset, can you show some evidence to support your answer?
a- New year's day 
b- November 8, 2016

2. Which page experienced the biggest decline in page visits during 2016?

3. Which page experienced the biggest increase in page visits during 2016?

4. Wikipedia pages could be written in several languages. How many languages are represented in this dataset? What proportion of the pages does each language represent? 
- Hint: One may infer which language a page is written in based on the page name
e.g. Special:Search_fr.wikipedia.org_all-access_all-agents is written in French and Special:Book_en.wikipedia.org_all-access_spider is written in English.


5. Based on the provided dataset, which day(s) of the week is/are the most popular for visiting wikipedia?

6. Based on the provided dataset, which day(s) of the week is/are the least popular for visiting wikipedia?

7. Based on the dataset provided, which device type is used more frequently for visiting wikipedia i.e. desktop or mobile devices?
- Hint: For some of the pages in the dataset, it is possible to distinguish whether the visits to the page came from a desktop or a mobile device.
For example, consider Barack Obama's wikipedia page:
* Barack_Obama_en.wikipedia.org_desktop_all-agents : these visits came from desktop devices.
* Barack_Obama_en.wikipedia.org_mobile-web_all-agents: these visits came from mobile devices.


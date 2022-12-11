### Table of Contents
1. [Introduction](README.md#Introduction)
2. [Business Task](README.md#Business-task)
3. [Data](README.md#Data)
4. [Processing and Cleaning](README.md#Processing-and-cleaning)
5. [Conclusion and Recommendations](README.md#Conclusion-and-Recommendations)

## Introduction

The project is a part of **Google Data Analytics Certification course capstone**. The scenario involves analysis of the trip data of Cyclistic bike share company.

The company has two models for availing service: individual passes which are called "casual" riders and annual subscriptions called "member" riders.
The company operates in Chicago with around 6000 bicycles at 700 stations.

Maximizing the number of annual members will be key to future growth as it ensures financial sustainability and customer retention. The insights can help devise effective marketing strategies aimed to convert more casual riders into annual members.

## Business Task

To **analyze historical bicycle trip data** in order to **identify trends**. Understanding how casual riders behave differently from riders with paid memberships. This *analysis will help executives* to make *decisions about marketing programs and strategies* to convert casual riders to riders with annual memberships.

> **Objective** : To clean, analyze and visualize the data to observe how casual riders use the bike rentals differently from annual member riders. 
## Data

* **Data source** : Public data from Motivate International Inc. (Divvy Bicycle Sharing Service from Chicago) under this [license](https://www.divvybikes.com/data-license-agreement).
* [Cyclistic’s historical trip data](https://divvy-tripdata.s3.amazonaws.com/index.html) (2013 onwards) available in `.csv` format. 
* **Our date range** : June 202013 to October 2022 (4.9 GB data)
***Data Organization & Description:**

* File naming convention: YYYY_MM

* File Type: csv format

* File Content: Each csv file consist of 13 columns which contain information related to ride id, rider type, ride start and end time, start and end location etc. Number of rows varies between 49k to 531k from different excel files.


## Processing and Cleaning

I used Excel, SQL and R for data verification and cleaning: Reasons: The 55 data sets combined will contain more than 14 million rows of data. Excel worksheet limitation is 1,048,576 rows. Moreover, some csv files could not uploaded to BigQuery for file size problems. Thus, R is used to perform all tasks from organizing, cleaning analyzing and visualizing data.

**Organizing Data.**

I have use Excel to merge some files.

We will Combine the 2nd Quarter data from 2016 month 04,05,06 through
Microsoft Excel.

![Excel](https://ibb.co/p33F8b2)

We also require to merge the data of 2015 Q3 month 07,08,09 this time we
will use SQL to do so.

![SQLite](images/Merging%202015%20Q3%20in%20SQLite.JPG)

*Futher Analysis is shown in above .rmd File please check it for further understanding.*
Google Data Analysit Capstone Cyclistic Project.Rmd


## Conclusion and Recommendations


The amount of time, frequency, and days of the week on which each group
peaks varies between annual members and casual riders:

-   Weekends are busiest for casual rides (plot3). It's very likely that they are city visitors who are visiting the sights, or that they are regular Chicago     residents who are enjoying a weekend bike ride. This is supported by the fact that the average ride time for casual riders (plot2) is longer and increases     on weekends.

-   Members typically ride for a shorter period of time than casual
    riders. This could be clarified by saying that the majority of the
    members commute to work on bicycles. This clarification would also
    shed light on why members only ride for brief periods of time. They
    travel daily commute, which is roughly the same distance and ride
    length every time.

-   (Plot 8). shows that ridership begins to increase in February (from
    Spring through Summer) and that it then begins to decline in August
    (from Fall through winter). The seasonal changes are what cause this
    correlation. More people begin to cycle as the weather begins to
    warm up and become more pleasant in February (the beginning of
    Spring), and the opposite is true as the weather turns cold and less
    pleasant around September (start of Fall).

-   More than 50% of the riders (plot 5) are annual members, indicating
    that the business has already attained a certain level of customer
    loyalty. This suggests a positive message, namely that the company
    will be able to persuade many casual riders to become members and to
    maintain the satisfaction of the new members.
    
**To see Recomendation Please read the .rmd file above**

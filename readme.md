# Bike-sharing Service Usage Analysis

### Case study done as part of the Google Data Analytics Professional Certificate.

#### March 2024.

This **summary** provides an overview of the problem, processes and key findings from the case study. For a detailed account, refer to the full report in the [report.md](/report.md) file.

## Overview

This case study explores the usage patterns of a San Francisco bike-sharing service, with the objective of informing a digital media marketing campaign designed to convert casual riders into subscriber members. The analysis is driven by data provided by Ford GoBike Share, available through the Google Cloud Public Datasets - accessible [here](https://console.cloud.google.com/marketplace/product/san-francisco-public-data/sf-bike-share). Utilizing tools such as Google Sheets, BigQuery, and Tableau, the study includes data gathering, cleaning, and analysis phases, resulting in three strategic recommendations.

## Goal

The main objective is to leverage usage data insights to assist the marketing team in developing their campaign, specifically by answering a key question they that have posed: How do casual riders and subscriber members use the service differently?

## Dataset


- The dataset features individual trip records, focusing on a one-year period with complete data. 
- The data was collected internally and is in good condition for analytical use. 
- Limitations include the absence of user ID tags, hindering the ability to link trips to individual behaviors precisely.

## Approach

- Using BigQuery, I cleaned and streamlined the dataset to focus on a manageable subset of over 300,000 records from the original dataset exceeding 2 million rows.
- I developed SQL queries to address data inconsistencies, particularly with station IDs, and refined date-time information for detailed temporal analysis.
- To address potential biases introduced by varying group sizes, the analysis was based on relative measurements instead of absolute values.
- Pivot tables created in Google Sheets facilitated dynamic manipulation and visualization of data trends.
- I employed Tableau to create the final visualization for sharing with stakeholders, building a dashboard that highlighted user behavior patterns comprehensively.

## Results and Insights

- Total Trip Counts: Subscribers contributed significantly more trips, totaling 277,389, compared to 33,460 trips by casual riders.
- Average Trip Duration: Casual riders' trips were longer on average, lasting 50.1 minutes, versus subscribers' average of 9.5 minutes. 
- Daily Activity Patterns: Subscribers' usage peaked during rush hours, with almost 70% of trips between 7-9 am and 4-6 pm. Casual riders showed a more even distribution of activity throughout the day, with a surge in the early afternoon, starting 70% of their trips between 10 am and 5 pm.
- Weekly Activity Patterns: Nearly 40% of casual riders' trips occurred on Saturdays and Sundays, contrasting with only about 5% of subscribers' trips during the weekends.
- Seasonal Variation: Both user groups increased usage during warmer months and decreased during the holiday season. Subscribers, however, showed more consistent usage throughout the year.
- Preferred stations: Over 34% of  trips for each group originate from their top 6 busiest stations, with Harry Bridges Plaza (Ferry Building) being the only common among both groups' top 6.

These results show a strong indication that subscribers primarily use the bike-sharing service for commuting purposes, while casual riders exhibit a pattern suggesting a more varied use of the service. Even though there may be some overlap in popular locations, each group has unique patterns in station usage. 

## Recommendations

The marketing team intends to convert users, using a marketing campaign based on digital media. With this in mind, here are my three recommendations for them:
- Target customers being active during rush hours and at the main stations used by subscribers. Emphasize the benefits they could take from commuting to work on a bike. They are either in a busy area or in a time of day that’s really busy. Leveraging these insights ensures that the marketing efforts are directed towards potential subscribers who are most likely to find value in frequent bike usage, similar to existing subscribers.
- Focus some of the campaign on periods when customers are the most active. That way you can reach a bigger audience and it increases the likelihood of engaging casual riders during times when they are more receptive to the idea of riding bikes. These periods are the weekends and during the warmer months of the year.
- Connect this data to the customer information database, if the team can link member IDs to the individual trips, they will be able to better understand user behavior based on their profile and deepen their knowledge on differences between customers and subscribers. 

## Conclusion

This study offered strategic insights into differentiating usage patterns between casual riders and subscribers in a bike-sharing service, guiding targeted marketing efforts. By focusing on data-driven recommendations, there’s a clear path forward for converting casual riders into subscribers, leveraging peak activity times and station preferences.

## Visualization

The resulting visualization, showcasing the analysis, is displayed below. This was created using a Tableau dashboard, primarily for practice rather than necessity. However, this dashboard, accessible [here](https://public.tableau.com/app/profile/lucas.zappe/viz/case_study_01/Dashboard1), allows for some interactive exploration of the data, with the capability to filter charts by subscription type to examine each group's data separately.

[![final viz](images/dashboard.png)](https://public.tableau.com/app/profile/lucas.zappe/viz/case_study_01/Dashboard1)

[**Back to Top**](#bike-sharing-service-usage-analysis)

[**Go to Full Report**](/report.md)




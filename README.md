# Kickstarting with Excel

## Overview of Project
Our client Louise recently utilized Kickstarter in attempt to fund production of her play *Fever*. While she came very close to achieving her funding goals, she ultimately fell short. 

### Purpose
In an effort to beter understand possible reasons why her fundrasing goal fell short, and how she could improve future efforts, Louise has asked that we perform an analysis of past Kickstarter campaigns. Utlizing Excel and a dataset of 8 years of kickstarter data, analysis pertinent to the aforementioned goal was performed. 

## Analysis and Challenges
Analysis of past Kickstarter campaigns was performed on specific subsets of the available data most applicable for understanding what contributes to a succesful kickstart campaign. Specifically, the outcomes of past plays funded through Kickstarter were looked at versus both their campaign launch dates, and the initial fundrasing goal set for each. 

### Analysis of Outcomes Based on Launch Date
![Theatre_Outcomes_vs_Launch](https://user-images.githubusercontent.com/81761879/115962784-f1be1180-a4ea-11eb-8ae5-0aa842b1e614.png)

The above chart illustrates the total number of succesful, failed, and canceled plays by month, over the course of roughly 7 years. 

### Analysis of Outcomes Based on Goals
![Outcomes_vs_Goals](https://user-images.githubusercontent.com/81761879/115962961-af490480-a4eb-11eb-9837-919c5608e43f.png)

The above chart illustrates the percentage of plays that were succesful, failed, or canceled based on their initial funding goals, over the course of roughly 7 years. Funding goals were broken down into subsets with a range of $5000. 

### Challenges and Difficulties Encountered

Fortunately, we did not encounter any major challenges in analysis of the above datasets. One small challenge was the need to transscribe the campaign start date from unix timestamps into traditional month/day/year format. This was achieved by a simple formula that divided the unix timestamp by the number of seconds in a minute, the number of minutes in an hour, the number of hours in a day, and then adding that total to the initial date of January 1st, 1970.  One other possible challenge that could have occured would have included a kickstarter campaign which had a very large initial funding goal that was also succesfully met. This would have presented a skewed positive outcome towards the higher range of succesful finding goals, but would have been based on a large outlier, and would have required the removal of these outliers before analysis. 

## Results

As can be seen in the theatre outcomes vs launch date, one of the biggest take aways from our analysis is that campaigns which launched during the summer months of May and June had sigfnicantly higher numbers of succesful funding versus other months. This might be a result of the warmer weather allowing more outdoor venues to be open for events, as well as children being out of school and families looking for activites during this period. This period not only had the most successful funding but also the most overall play kickstarters in general. Conversely, we can see the winter months Novevember and December proved the least succesful for succesful funding. However, it is interesting to note that the overall failure rates were fairly stable throughout the year with only minor fluctuations. Overall, Louise would have the best chance of success having launched in the Summer months. 

In relation to the outcomes vs funding goals, its fairly obvious that as funding goals increase, the chance of failure also increased. Plays with funding goals of less than $5000 had at least a 72% chance of success. The fact this data set was so large, 720 plays had $5000 or less as their funding goal, provides further confidence this finding is valid and reliable. Interestingly, there is a small spike in succes rates from the $35000 to $45000 range. However, these outcomes are based on an incredibly small data set of only 9 plays, which indicates we should interpret these results as not being as reliable for extrapolation. Overall, if Lousie can keep her funding goal under $5000, she stands the best chance of succesfully funding her play. 

## Limitations and Future Analysis 

Overall, there were a number of limitations specific to this data set. Most importantly, how the kickstarter was marketed was limited and not analyzed. While factors such as wether it was spotlighted, and/or a staff pick were available, this was not analyzed in terms of outcome. Knowing more granular marketing information such as what media was used to promote the kickstarter would also have been valuable information to analyse. In relation, Kickstarters are known for their incentives based on funding goals met, or individual funding levels. This information is completely absent in the data set. All of this information could have provided more insight into what contributes to succesful campaigns. 

Specific to the available data, future analysis that looked at success rates versus staff pick and spotlight would be valuable. In addition, looking at the outcomes of plays versus launch dates as a percentage of success vs failure, instead of total counts of each, would give more relevant insights. Finally, analysis of the average contribution could be looked at in order to formulate a range for different incentive levels.

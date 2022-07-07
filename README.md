# Kickstarter-Assignment-
Kickstarter Assignment for Module 1 Challenge
## Overview and purpose of Projects
---
Louise attempted to fundraise a play by the name of “Fever”, unfortunately she fell short of her goal and the play could not be financed. The purpose of these analyses is to find a correlation between either the release date or the goal amount to the success of fundraising the play. The purpose in doing so will hopefully grant insights on what creates a successful fundraiser for all of Louise’s future plays. 
## Analysis and Challenges
### Analysis of Outcomes Based on Launch Date
---
In order to complete this analysis, I first created an excel formula to convert the launch date and deadline columns into a readable and useable date format. From there I was able to create a “years” column to organize the Year in which each entry launched. Once all of my data was in order, I was able to create a pivot table. In the Pivot Table, I sorted it by putting the date created in the Rows tab, outcomes in both the Columns tab and the Values tab, and finally filtering with parent category and years. From there I was able to create a pivot chart with the results that the pivot table gave me which I was able to create a line graph to show the trend of successful kick-starters by what time of the year they are released. The End result of the Pivot chart was:
![Theater_Outcomes_vs_Launch](Resources/TheaterOutcomesvsLaunch.png)

---
### Analysis of Outcomes Based on Goals
---
For the Analysis of the outcomes based on Goals, I used the command 'CountIf' followed by logic to explain the conditions in which the program will count certain values. The value for successful kickstarters that were under $1000 was written by the following code
=COUNTIFS('kickstarter data'!$D:$D, "<1000",'kickstarter data'!$F:$F, "successful",'kickstarter data'!$P:$P, "plays")
The rest was essentially completed the same way with the percentage totals being calculated based on the counted results. The final Pivotchart looked like:
![Outcomes_vs_Goals](Resources/Outcomes_vs_Goals.png)
---
---
### Challenges and Difficulties Encountered
---
Overall, I did not have too many issues with the assignment and performing the analyses. I was a little confused with the outcomes based on goals with the countifs feature however after looking at some online help resources, I was able to understand what I needed to do and 
completed the analysis.
---
## Results
- What are two conclusions you can draw about the Outcomes based on Launch Date?
---
One conclusion from outcomes based on launch date is that the summer months projects are more likely to succeed compared to the winter months. Additionally, another conclusion that can be made is that the failure rate is relatively consistent regardless of what time of year it is (except for January which seems to be an outlier). 
---
# What can you conclude about the Outcomes based on Goals?
---
When looking at the Outcomes based on Goals, we can conclude that projects with smaller goal sizes have a much easier time of reaching their goal than projects that are a lot more expensive.
---
# What are some limitations of this dataset?
---
For the outcomes based on the launch date analysis, the failure rate for the month of January was suspiciously large, I suspect that there was an error in the dataset that caused this outlier to occur.
# What are some other possible tables and/or graphs that we could create?
---
We could create another pivot table where we sort successful campaigns by region (Country) so get insights on different regions and what regions are more engaged to supporting theatres and plays. 

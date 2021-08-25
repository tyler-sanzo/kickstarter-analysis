# Kickstarting with Excel

## Overview of Project
Using data from Kickstarter to provide meaningful analysis on what makes a project successful or unsuccessful.

### Purpose
Louise is looking to raise money for her play through Kickstarter, a crowdfunding platform dedicated to help bring creative projects to life. With the help of excel, we are tasked with using a variety of data pulled from thousands of Kickstarter projects to help Louise succeed with her campaign.

## Analysis and Challenges
The base dataset we were give was a table of kickstarter projects that summarized each project by giving financial information, when the campaign started/ended, the category and subcategory, and the location of the project. Having all of this information is useful because it allows us to make more accurate analyses by drilling down the data to only projects related to Louise's. 

### Analysis of Outcomes Based on Launch Date
Using the data provided about the start dates of the kickstarter projects can give us an idea on when successfully funded projects are started. A pivot table was created  and used to plt the number of outcomes for each series (successful, failed, canceled) against months of the year. The most appropriate graph for this was a line graph as we want to see how these outcomes trend throughout the year.

### Analysis of Outcomes Based on Goals
To further assist Louise, we were able to use the amount of funding each project was asking for and the outcome of the project to give her a better understanding on an appropriate amount of funding she should ask for in order for her project to succeed. Goal amounts were binned into 12 ranges and the counts of all 3 outcomes were calculated for each of these ranges. 

### Challenges and Difficulties Encountered
One challenged faced in the outcomes based on goals analysis was setting up the COUNTIFS function such that goal amount bins were created based on certain dollar ranges. To overcome this and clean up the formula, two columns were created with the lower and upper bound of each range for reference in the formula. 
## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
Looking at the chart made comparing the launch date and outcome of the kickstarter, we can conclude that theater projects are far more likely to be successfully funded as summer approaches. Specifically, those launched during month of May see a high likelyhood of success compared to the others. On the flipside, theater projects do not do well as the year comes to an end. For instance, December was the only month where less than half of the total projects ended up successful. 

- What can you conclude about the Outcomes based on Goals?
The chart created using the goal amounts and comparing the number of successful and failed plays shows us that as the asking amount increases, the chance of success tends to decrease. The data shows that Kickstarters with a goal of less than 5000 tend to yield the highest amount of success as we see a sharp drop in success rate at ranges beyond this.

- What are some limitations of this dataset?
Although the data provided did allow us to give some analysis to help Louise better plan her campaign, there were a couple limitations. One limitation which can be seen on the outcomes based on goal amounts chart is the fact that over 90% of the goal amounts for kickstarters for plays were under 15000. This means that the analysis for projects in the upper ranges cannot be used to make conclusions as the sample size was too small in comparison. One other limitation for the same analysis was the fact that these goal amounts were binned together but the currencies were not uniform across. This means that there could be some projects that, when converted to USD, would fall into a different bin and show us results that look different than our initial chart. 

- What are some other possible tables and/or graphs that we could create?
Another graph that could provide additional insight for Louise would be similar to the outcomes based on launch date but instead we could use the total campaign time. While using the launch date is very helpful and the conclusions seem to make sense, this chart doesn't tell us how long the campaign lasted. It would make sense that a campaign that lasts a year has a higher chance of being "successful" by the time it ends compared to a campaign is only open for a week. Using the start and end date we could calculate the total number of days and use this to analyze the success rate of play campaigns based on how long the crowdfund is open. 
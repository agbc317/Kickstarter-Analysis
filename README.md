# Kickstarting with Excel

## Overview of Project

### Purpose

The data for this analysis comes from Louise who has recently fundraised for her play Fever on Kickstarter and the purpose of this Analysis is to gain a better understanding of what makes a successful Kickstarter campaign. 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

For this piece of the challenge I first created a Pivot Table on a New Sheet which I renamed Theater Outcomes by Launch Date. I then added Filters for Parent Category and Years. For the Rows I added Date Created Conversion which has the conversion of the original date column from the data we were given. I then added Count of outcomes to the Values section and outcomes to the Columns section to get the full Pivot Table. To get the final version of the Pivot table that was used for the final chart, I filtered by Parent Category to only show theater outcomes. I then inserted a line chart with the months of the year on the X-Axis and the number of outcomes on the Y-Axis. This created the Theater_Outcomes_vs_Launch.png that shows the results of this Pivot Table.

### Analysis of Outcomes Based on Goals

For this piece of the challenge I first created a New Sheet which I renamed Outcomes Based on Goals. I then added the different Goal categories that we were given in the instructions in the first column. I then created the columns for Number Successful, Number Failed, Number Canceled, Total Projects, Percentage Successful, Percentage Failed, Percentage Cancelled. 
For the Number Successful column I used the formula "=COUNTIFS(Kickstarter!R:R,"plays",Kickstarter!$F:$F,"successful",Kickstarter!$D:$D,"<='maximum'",Kickstarter!$D:$D,">='minimum'")" replacing maximum and minimum for each row to gain a count of the number of campaigns for plays in the range that were successful. 
I then repeated this for the Number Failed and Number Canceled columns but replaced Kickstarter!$F:$F,"successful" with the correct value for the column.
For the Total Projects column I used the Sum function to add up the Number of Successful Failed and Canceled Kickstarters in each row. 
For the percentage columns I used a formula to divide the number of either successful, failed, or canceled projects by the total number of projects. 
After I had filled out this table I highlighted the Goal, Percentage Successful, Percentage Failed, and Percentage Canceled columns and inserted a line chart titled, Outcomes Based on Goals which I then saved as an Image. 

### Challenges and Difficulties Encountered

For this Challenge I encountered a few difficulties but they were all easy to fix. My biggest problem was with my formula to count the number of cancelled projects where my problem was that I had misspelled "canceled". One of the other difficulties I encountered was too many rows in my pivot table that I hadn't realized had been added. Luckily for all of the difficulties I encountered I was able to figure out the problem and move on quickly. 

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?
It seems from the chart that was created that there is a higher number of theater kickstarters launched in the months of May and June. It seems that there is also a higher number of these projects that are successful which would suggest that this is a good time to laugh one of these projects and also that people have realized this and have started to launch more of their projects during these months. 

- What can you conclude about the Outcomes based on Goals?

From the Outcomes based on Goals data we can conclude that as the goal of a kickstarter projects increases, the likelihood of it being successful decreases. There is an interesting increase in the likelihood of a successful campaign between 35000 and 45000. This could be due to campaigns in this budget being pushed more by their marketers or it could be some kind of externality that explains this change. 

- What are some limitations of this dataset?

Some limitations of this dataset include a lack of information about who was running the campaigns and the amount that the links for these campaigns were shared.

- What are some other possible tables and/or graphs that we could create?

Some possible graphs that could help with understanding of this data set could be one that shows the percentage of successful failed and canceled campaigns based on launch month. Another table that could be helpful would be one that shows the relationship between the number of backers and goal and whether or not the campaign was successful.

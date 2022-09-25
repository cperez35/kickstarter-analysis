# Kickstarting with Excel

## Overview of Project

### Purpose
Louise wanted to know how different campaigns fared in relation to their launch dates and their funding goals.
I completed an analysis to visualize campaign outcomes based on their launch dates and their funding goals.

## Analysis and Challenges
This assignment consists of two technical analysis deliverables and a written report to deliver your results.
    
- Deliverable 1: Outcomes Based on Launch Date Chart

- Deliverable 2: Outcomes Based on Goals Chart

- Deliverable 3: A written analysis of the results (README.md)

### Analysis of Outcomes Based on Launch Date

Created a pivot table and graphs in Excel to visualize campaign outcomes ("successful," "failed," and "canceled") based on launch date.

A pivot table named "Theater Outcomes by Launch Date" contains filters for categories and year. Filtering out the data to only show "theatre"results in the parent category we then had to group the rows to display the values by month and create columns to show succesful, failed and canceled outcomes. Then created a line graph with markers to show results. 

[Theater Outcomes vs Launch Date](../OneDrive/Desktop/Class%20Folder/Analysis%20Projects/Crowd%20Funding%20Analysis/resources/Theater_Outcomes_vs_Launch.png.png)

### Analysis of Outcomes Based on Goals
Created a new sheet named "Outcomes Based on Goals" and used the "COUNTIFS()" function in excel to  visualize the percentage of successful, failed, and canceled plays based on the funding goal amount. Then I used the SUM() function on each row to add the "Number Successful," "Number Failed," and "Number Canceled" columns to populate the "Total Projects" column. We then used that total and divided by the number of succesful, failed and canceled campaigns and used a line graph to show the results. 



[Outcomes vs Goals](../OneDrive/Desktop/Class%20Folder/Analysis%20Projects/Crowd%20Funding%20Analysis/resources/Outcomes_vs_Goals.png)

### Challenges and Difficulties Encountered

During the analysis of outcomes based on goals we had to create a countifs formula that filtered from the original data set:
- Successful, Failed and Canceled campaigns (column F:F)
- Only show results for the subcategory of 'Plays' (column R:R)
- Classify the results based on goal ranges column (D:D)

The result is a formula that looks like this 

- =COUNTIFS(Kickstarter!$F:$F,"=successful",Kickstarter!$R:$R,"=plays",Kickstarter!$D:$D,">=1000",Kickstarter!$D:$D,"<=4999")

To produce a result of successful plays that made from $1000 to $4999. I had a challenge formatting this formula in a way the yielded the appropriate result. I solicited the help of AskBCS. 


## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date? 
  
  - You can conclude that:
  
    * May is month with the most successful outcomes for theatre
    
    * October is the least favorable month because of a downward trend in successful campaigns as well as an increase in failed ones.  

- What can you conclude about the Outcomes based on Goals?
   
   - Because there were no canceled plays, the successful and failed campaigns share an inverse relationship on the line graph. 

- What are some limitations of this dataset?

   -  More info regarding failed and canceled results to optimize kickstarter outcomes.
   - Another useful analysis might be to run a countifs formula for the "pledged" amounts to see if there is any correlation between successful campaigns and the amounts pledged. 




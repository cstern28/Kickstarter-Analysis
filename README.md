# Kickstarting with Excel

## Overview of Analysis of Kickstarter Campaign Project
We wanted to analyze the status of completed campaigns. 

### Purpose 
The purpose of the Kickstarter Analysis is to help Louise determine whether there are specific factors that help make a crowdfunding campaign successfull.

## Analysis and Challenges
I performed my analysis by starting to create a pivot table following the steps outlined. 

Overall, two graphs were created from the Kickstarter data. 

### Analysis of Outcomes Based on Launch Date
For the first deliverable, I created a few new columns called Date Created Conversion and Years. Then, I created a pivot table to understand theater outcomes by launch date. The, I used the pivot table to create a line chart, which shows the number of successful, failed, or canceled projects by month (Refer to line graph image below).
![image](https://user-images.githubusercontent.com/102467249/164909418-4187887e-1d5f-411e-94d6-fbe173c42c50.png)

### Analysis of Outcomes Based on Goals
For the second deliverable, I created a new worksheet called, "Outcomes Based on Goals". In the sheet, I calculated using SUMIF to determine the total projects that were successful, failed, and canceled based on the campaign goal range and only for the "plays" subcategory (Refer to the line graph below, called "Outcomes Based on Goal"). 
![image](https://user-images.githubusercontent.com/102467249/164909692-b5f480b6-c893-4dd9-938e-48e9b1d72659.png)

### Challenges and Difficulties Encountered
I realized that my pivot table subtotals were inaccurate and I had to re-do my kickstarter analysis by reworking through lessons 1-5. Luckily, after completing a second time, I had the same subtotals as the example shown in the instructions. Another challenge, was creating the SUMIF formula to count the number of campaigns that were between a certain goal amount, status of campaign, and whether the campaign was related to a play. I had trouble writing the SUMIF formula to include the required range accurately, but was able to figure it out by creating a new column, called "Max Goal". Here is my formula used for rows 3 5o 12: "=COUNTIFS(Kickstarter!$D:$D,"<"&$B3,Kickstarter!$F:$F,"successful",Kickstarter!$R:$R,"plays")-SUM(C$2:C2)". I separated the two ranges by writing the sheet referenced twice and using commas between the two criteras.

## Results

For the first deliverable, "Outcomes Based on Launch Date" chart, I concluded that the successful campaigns were started in May and in June. In May, there were 111 successful Theater campaigns and in June, there were 100 successful Theater campaigns. Also, I noticed that there were few campaigns overall that were canceled. The highest number of canceled play campaigns occurred in January with only 7 canceled campaigns.

For the second deliverable, "Outcomes Based on Goals" chart, I concluded that the campaigns with a goal of less than $1,000 were the most successful, with 75.8% success rate percentage. The next most successful campaigns set a goal of less than $5,000 with a 72.7% success rate percentage. In additional the campaigns that were more likely to fail had a very high set goal or greater than $50,000 and those campaigns had 88.2% failed rate percentage.

Although some conclusions could be drawn, there was a limitation to the data set, being that majority of the data set included play campaigns with limited data for other subcategories. It appears most successful campaigns are for plays, however the data does not include many data points for successful campaigns in other subcategories. Is that really the case or was the data limited to mostly play campaign data? I would recommend addition data on other subcategory campaigns, such as food, games, journalism, and publishing to make more pivot tables, such as subcategory/parent categories analysis and line graph analyses, such as status and parent categories.

The overall conclusion drawn, is that campaigns with high, ambitious fundraising goals were not as successful as campaigns with reasonable, realistic fundrasiing goals.

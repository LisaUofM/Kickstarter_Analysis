# Kickstarting with Excel

## Overview of Project
"Theater" is the most popular category among kickstarter campaigns and "Plays" is the most popular subcategory within "Theater." (See "Category Statistics" and "Subcategory Statistics" tabs in "An Analysis of KickStarter campaigns": https://github.com/LisaUofM/Kickstarter_Analysis/issues/4#issue-1087085269). Our client Louise conducted her own kickstarter campaign for her play "Fever," and had very positive outcomes. She has requested further insight into the performance of other campaigns within her industry/sector (or, Category/Subcategory).

### Purpose
The purpose of this analysis is to provide additional data perspectives on the Category/Subcategory "Theater/Plays" that demonstrates how certain conditions can drive performance. To do this, we specifically look at "Theater Outcomes By Launch Date" and "Theater Outcomes Based on Goals." 

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date
A pivot table was created to organize and quantify the Kickstarter campaign data with fields "Parent Category" and "Years" selected as the filters. (Parent Category was filtered to "Theater" and Years was unfiltered to include all years in the kickstarter data). The field "Outcomes" was selected as column headers and "Data Created" was selected for row headers. "Outcomes" was selected again for the Values field list. See screenshot "Outcomes by Launch Date Pivot." https://github.com/LisaUofM/Kickstarter_Analysis/issues/7#issue-1087237367

### Analysis of Outcomes Based on Goals
(All screenshot references can be found in this link: https://github.com/LisaUofM/Kickstarter_Analysis/issues/5#issue-1087145148) 

#### Data Structure/Organization
Kickstarter campaign goals for "Theater/Plays" were categorized by outcomes: "successful," "failed," and "canceled" (See Screenshot Item #1) while the range of goal dollar amounts for each campaign, from "0" to "200,000." were broken into $5000 segments, starting at $1,000-$4,999 and continuing with $5,000 to $9,999 ... through $45,000 to $49,999. The lowest and highest increments were an exception to these segments, with the lowest being captured as "Less than 1000" and the highest reflected as "Greater than $50,000." (See Screenshot item #2) 

#### Data Aggregation 
The totals for each segment were captured using excel "countifs" formulas with conditions that identify the subcatgory, outcome and $ segment of the goal. (See Screenshot item #3). 

The total count of projects by goal segment were captured by summing the counts across the outcomes. (See Screenshot Item #4)

For an indepth look at performance outcomes, percentages of outcome by Total Project count for each dollar segment were calculated. (See Screenshot Item #4)

#### Data Presentation
For visualization of the data, a line graph capturing performance (successful, failed, canceled) by outcome/total % and each dollar segment was created. https://github.com/LisaUofM/Kickstarter_Analysis/issues/3#issue-1086335490


### Challenges and Difficulties Encountered
There were no challenges or difficulties encountered in putting together this analysis. The raw data extrect was in excel and all the cells were clean and consistently formatted. In the future, if further analysis in the form of pivot tables and graphs is needed, excel as a tool for data analysis, is not the best option, as its performance declines with an increase in file size.

## Results

### What are two conclusions you can draw about the Outcomes based on Launch Date?  
1. The number of successful outcomes and the number of failed outcomes is positively correlated with overall fundraising activity. Apart from the months of November and December, spikes and dips in the numbers of successful and failed outcomes follow the same pattern as overall fundraising activity. 
https://github.com/LisaUofM/Kickstarter_Analysis/issues/2#issue-1086335142
2. Since we know that May-June sees the most fundraising campaign activity and that successful outcomes are positively correlated with overall activity, May is the best time to launch a theater fundraising campaign. 

### What can you conclude about the Outcomes based on Goals?
The campaign goal segments most consistently driving a successful outcome are 1. "Less than 1000" 2. "1000-4999" and 3. "35,000-39,999" tied with "40,000 to 44,999".  At these segments, we see the highest percentage of successful campaigns and the lowest percentage of failed campaigns. See Outcomes_vs_Goals_Conclusions: https://github.com/LisaUofM/Kickstarter_Analysis/issues/6#issue-1087184397

### What are some limitations of this dataset?
The dataset for Theater Outcomes By Launch Date is limited in that it is missing the correlation coefficient to support the conclusion that the outcomes are positively correlated with activity. The dataset for Outcomes Based on Goals does not include pledge data and an analysis of successful campaigns that exceeded their goals. 

### What are some other possible tables and/or graphs that we could create?
An additional table that displays theater outcomes and the correlation coefficent to overall activity could offer insight into what drives a successful campaign. A line graph displaying outcomes based on Goals and Pledges by goal amount segments would show where pledges exceeded goal amounts and offer another insight into successful fundraising decisions. 
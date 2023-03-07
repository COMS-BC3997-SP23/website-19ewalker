---
layout: default
title: Project Week 7
parent: Updates
---

## Project Week 7

Before jumping straight into the income and neighborhood data, I realized it would be helpful to get counts for the total number of calls by month, year
since that's one of the hypotheses I'm interested in exploring!

I wrote a for loop to parse the Created_Date column in order to return the month + year of a given call in the format XX 20XX and created a new column called 
Created_MonthYear. If a given call was created on 01/01/2018 12:04:05 AM, the corresponding value in Created_MonthYear for that row would be 01 2018.
I could probably do a switch case to reformat with the month (ex: January, instead of 01), but I did not do so yet because I was **lazy**. 

After parsing that info, I created a table that ranked the months with the most calls in descending order, and I also created a chart in MatPlotLib in order to
visualize how call frequency changed over the five year period I selected! This graph is pictured below.

![image](https://user-images.githubusercontent.com/44076192/223291057-dff0db0b-f8b0-4353-99af-6576d020c6f7.png)

I was actually pretty surprised by this graph. While March and April 2020 call frequency are both relatively similar to levels in 2019, call frequency starts exploding in May 2020 and reaches peak heights in summer of 2020. This call frequency also doesn't seem to follow normal patterns during COVID in general. Normally, the number of noise complaints peak in the summer and decline in the winter. However, we're able to see from this graph that call frequency in December 2020 and February 2021 outnumber those in July 2019. 

Just to test if I could create chronological call frequency graphs based on neighborhoods (or boroughs, zip codes, etc), I made a similar graph solely based on 311 noise complaint frequency in Central Harlem - Morningside Heights, which is the neighborhood in which Columbia is located.

![image](https://user-images.githubusercontent.com/44076192/223292383-9cd89425-ed82-4ec9-8aa4-6509605bd953.png)

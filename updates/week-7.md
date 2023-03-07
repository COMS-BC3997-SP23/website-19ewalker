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

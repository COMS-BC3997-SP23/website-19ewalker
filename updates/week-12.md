---
layout: default
title: Project Week 9
parent: Updates
---

## More Temporal Analysis

### Hours of Day
Somehow I forgot to measure noise complaint frequency by hour of the day, so I took care of that quickly. I made a new function to slice the 'Created_Date' column in order to get the hour, and I made a graph in MatPlotLib to display the frequency of 311 noise complaints by hour of the day.

![image](https://user-images.githubusercontent.com/44076192/233664845-a9e775ad-4a95-4f01-8a04-d426e581fad2.png)

Not that surprisingly, calls were most frequent during 11 PM, 10 PM, and midnight respectively.

## Days of Week

I also wanted to check out noise complaints by hour of the day, so I used the datetime library to convert my date strings into datetime objects and 
convert the datetime into a day of the week. I then plotted this in MatPlotLib (I finally learned how to change the x axis labels!)

![image](https://user-images.githubusercontent.com/44076192/233673325-beeab6a0-e1f2-4817-9a8d-d0d50bfe7f0e.png)

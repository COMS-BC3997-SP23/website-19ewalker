---
layout: default
title: Project Week 8
parent: Updates
---

## Project Week 8 (aka Check-In Time)

Here's a brief rundown of what I've been up to with this project. My goal is to analyze differences in 311 noise complaint activity in New York City 
that occurred during the COVID-19 pandemic. 

I came in with a couple of hypotheses that I wanted to explore. 

1. I believed that NYC’s 311 Call Center received on average **more complaints about noises** in the first three months of the pandemic than the Call Center received in the same period during 2019.
2. Meanwhile, I believe the call center will receive on average **less complaints about commercial, vehicle, and street/sidewalk noise** in these first three months compared to the same period in 2019.
3. During this three month period, I believe that **low-income zip codes will experience/report more monthly noise complaints** on average compared to non low income zip codes.

I sourced my 311 noise complaints from the 311 Dataset from NYC.gov, choosing to only include noise complaints between January 1 2018 and December 31 2022 in order to have a wider timeframe to analyze. After cleaning this data, I performed some exploratory statistics to better understand the patterns I was working with. By the way, I'm currently using Python (mainly Pandas / MatPlotLib) for all of my data analysis!

### Exploratory Statistics

The most common 5 types of noise complaints in the period were Noise - Residential, Noise - Street/Sidewalk, Noise - Vehicle, Noise, and Noise - Commercial. The most common 5 noise complaint descriptions were Loud Music/Party, Banging/Pounding, Loud Talking, Car/Truck Music, and Noise: Construction. As you can see below, the loud music + party complaint is the most common description by a mile.

Next, I knew this project was going to be largely focusing on changes in noise complaint call frequency over time, so I thought it would be helpful to create a graph of the number of noise complaints made in New York City during each month in the five month period I was studying (January 2018 - December 2022). I believe this graph is a pretty useful tool for identifying some key patterns for noise complaints, demonstrating both the periodic nature of noise complaints and the large increase in calls which begins in Summer 2020 and never seems to decline to pre-pandemic levels.

![image](https://user-images.githubusercontent.com/44076192/226217841-66d296fc-a348-4d7c-9e14-849fdccb0c8d.png)

In addition to temporal changes, I was interested in gathering information about the differences in noise complaints across zip codes and neighborhoods.
While the 311 dataset already includes a zip code category, I thought it was important to add neighborhood labels to each noise complaint. In order to identify neighborhoods by zip codes, I utilized the NYC United Hospital Fund Neighborhood Index which aims to match zip codes to neighborhoods.

After labeling most data entries with a neighborhood, I found the top 5 neighborhoods with the most noise complaints between January 2018 and December 2022 were Washington Heights / Inwood, the Northeast Bronx, Crotona - Tremont, Fordham - Bronx Park, and Bedford-Stuyvesant - Crown Heights. Meanwhile, the 5 neighborhoods with the least noise complaints were Canarsie - Flatlands, Sunset Park, Stapleton - St. George, Southeast Queens, and Rockaway. Repeating the process for zip codes, I found that 9 of the 10 zip codes with the most noise complaints were in Upper Manhattan and the Bronx.


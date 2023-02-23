---
layout: default
title: Project Week 5
parent: Updates
---

## Project Week 5

### Research Questions and Hypotheses
In my research, I’m interested in assessing how noise complaints shifted in New York City during the pandemic and in comparison to pre-pandemic periods.
- I believe that NYC’s 311 Call Center received on average more complaints about residential noises in the first three months of the pandemic than the Call Center received in the same period during 2019. 
- Meanwhile, I believe the call center will receive on average less complaints about commercial, vehicle, and street/sidewalk noise in these first three months compared to the same period in 2019. 
- During this three month period, I believe that low-income zip codes will be more likely to experience and report monthly noise complaints on average compared to medium-to-high-income zip codes.

I plan to source this data on low-income vs medium- and high-income zip codes using Census data on median household income by zip code.

In addition to checking out some of these hypotheses, I want to use this dataset as a starting point to tackling some different big data problems. For example, I think it could be really cool to do some prediction of type of noise complaint you'd likely experience in a given zip code at a given time of day. It could also be very cool to do some data visualizations of how call frequency varies over time. I'm still brainstorming things, but exploring this dataset has me excited for this project!

### Preliminary Data Analysis
In addition to brainstorming research questions, I've also been performing some preliminary analysis on my dataset to clean it up and get a sense of the most common complaints. I referenced the Jupyter notebook of a [similar project on 311 Data](https://nbviewer.org/github/oikonang/social_data_visualization/blob/master/Final_Project/Preliminary%20Analysis.ipynb) to help guide me when cleaning this dataset.

I started with cleaning my dataset. My data file was taken from the NYC Open Data database for 311 calls, and it is filtered to include only complaints whose Complaint Type mentions Noise, and between dates 13 February 2018 and 13 February 2023. Next, I loaded it into Python and dropped all irrelevant columns from the dataset so that all that remained were "Created Date", "Closed Date", "Complaint Type", "Descriptor", "Incident Zip", "Borough", "Latitude", "Longitude", and "Location". Next, I removed any rows with N/A info. This cleaning left me with 3179779 rows and 9 columns.

Next, I wanted to grab the unique categories for Complaint Type and Descriptor, just to get a general sense of the types of complaints. In this dataset, there were 9 unique complaint type categories that were reported with the following frequency (in most to least order):

**Most Common Noise Complaint Types**

1. Noise - Residential: 1,598,390 complaints
2. Noise - Street/Sidewalk: 714,582 complaints
3. Noise - Vehicle: 306,675 complaints
4. Noise: 250,478 complaints
5. Noise - Commercial: 244,588 complaints
6. Noise - Park:	32,704 complaints
7. Noise - Helicopter:	25,735 complaints
8. Noise - House of Worship:	5,919 complaints
9. Collection Truck Noise:	708 complaints

Below is a simple graph to visualize these complaint frequencies. 

<img width="855" alt="complaint_freq" src="https://user-images.githubusercontent.com/44076192/220824764-5ecb6721-5f65-4123-9e0a-4f0b4b9cda36.png">

Meanwhile, the top 10 complaint descriptions were as follows. My favorite new tidbit is that noise from ice cream trucks are the 14th most common complaint. 

**Top 10 Noise Complaint Descriptions**
1. Loud Music/Party: 1,903,334 complaints
2. Banging/Pounding: 418,678 complaints
3. Loud Talking: 233,756 complaints
4. Car/Truck Music: 200,128 complaints
5. Noise: Construction Before/After Hours (NM1): 103,688 complaints
6. Car/Truck Horn: 70,689 complaints
7. Engine Idling: 51,569 complaints
8. Noise: Construction Equipment (NC1): 36,253 complaints
9. Noise, Barking Dog (NR5): 31,436 complaints
10. Loud Television: 24,704 complaints

Here's another simple graph to visualize specific noise description frequencies.

<img width="855" alt="descriptor_freq" src="https://user-images.githubusercontent.com/44076192/220824785-50dabc52-bc1e-4858-acda-b415897fdad4.png">

Finally, I want to share some quick stats on the number of noise-related calls received over the period February 2018 - February 2023. Here is some quick info on the stats surrounding noise-related calls in those years.

- February 13 to Dec 31, 2018: 397,563 calls
- January 1 to Dec 31, 2019: 471,402 calls
- January 1 to Dec 31, 2020: 798,989 calls
- January 1 to Dec 31, 2021: 745,739 calls
- January 1 to Dec 31, 2022: 713,990 calls
- January 1 to February 13, 2023: 52,096 calls

We'll have to ignore the 2018 and 2023 data in this context since those aren't full years, but we can start to see that noise-related complaints increased by 70% from 2019 to 2020. I'm excited to keep exploring this data and see what else can be found in the coming weeks!

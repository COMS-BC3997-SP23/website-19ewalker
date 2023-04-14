---
layout: default
title: Project Week 10
parent: Updates
---

## Hypothesis Testing

In this section of my project, I am planning to test whether there was 

**(1)** a statistically significant increase in 311 noise complaint calls during the first three months of the pandemic compared to the same period in 2019, and

**(2)** a statistically significant decrease in commercial, vehicle, and street/sidewalk noise in these first three months of the pandemic compared to the same period in 2020 and a statistically significant increase in residential noise.

### Hypothesis 1

For this hypothesis, I conducted a paired t-test to compare the mean calls per day in the March 1 to May 31, 2019 period against the same period in 2020. 
A paired t-test is a significance test used when we want to examine the difference between two variables for the same subject, often when separated by time. Because we are examining 311 noise complaints in the same region over two different periods of time, this seemed like a natural fit.

To clean my data, I wrote a function to add a noise complaint date (not just month and year) that excluded time and then aggregated the noise complaints
by date. To narrow this down to the specific period, I only looked at dates between 03/01 and 05/31 in the years 2019 and 2020. 

Next, I entered the number of calls for each day of each period into two arrays and used the T-Test Rel function in the Scipy Stats library to test
these two sets for a statistically significant difference. I found a T-statistic value of -3.539 and a P-Value of 0.0006348, indicating that **there is
a statistically significant increase** in the number of 311 noise complaints during the 2020 period, compared to the same period in 2019.

![image](https://user-images.githubusercontent.com/44076192/232148063-ba1091cd-d1ff-4710-aa1d-7af6e4ef462b.png)

### Hypothesis 2
For my second hypothesis, this would require repeating the same paired T-test process on four different types of noise complaints: commercial, vehicle, 
street/sidewalk noise, and residential.

#### Commercial Noise

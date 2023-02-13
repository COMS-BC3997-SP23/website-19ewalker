---
layout: default
title: Project Week 4
parent: Updates
---

## Project Week 4

This week for my project, I decided to spend some time on literature review. Since the 311 dataset is quite large, I knew I wanted to narrow down my research to a particular subset of query. After some consideration of the types of possible 311 complaints, I decided to focus on changes in noise complaints throughout New York City over the course of the pandemic.

### Background Research

During my background research, I chose to focus on the background of 311, trends in 311 calls / noise complaints during the pandemic. I plan to do more research into the different phases of the pandemic in New York City next week. Below are some of my main takeaways.

**311 Calls**

In New York City, the 311 Call Center is a nonemergency service line created to obtain and report information for residents. The 311 non-emergency call system was initially built around the country to relieve the congestion in the 911 emergency system from non-emergency calls. Issues raised in calls can range from residential noise to plumbing problems. Beyond revealing some information about the issues in a community, 311 data can illustrate how a community function. For instance, 311 calls for interpersonal problems such as noise are a sign that those in the community are unwilling or unable to resolve local problems themselves.

Studying 311 datasets has a range of advantages and disadvantages. Importantly, 311 datasets are typically made widely available and contain high levels of detail. However, 311 callers are not evenly distributed across all zip codes. Typically, certain zip codes and demographics are more likely to utilize the service. For instance, a study of 311 calls over social distance violations in the early pandemic demonstrated that Black and Hispanic communities would be less likely to call in these violations. Additionally, a potential confounding variable can be overactive users who dominate the local calls in a zip code. Finally, while these calls provide geolocation, information about the caller's identity is not available.

**Pandemic 311 Behavior**

To begin, it appears apparent that 311 usage increased during the beginning of the pandemic. A previous study found that the NYC 311 call center received 17% more calls between March 28th and September 5th, 2020 than during the same period in 2019. 

In terms of noise, London saw significant increases in noise complaints from construction and neighbors, although housing and demographic factors played a more significant role than actual exposure to road and rail traffic noise. Due to these increases, some city councils in the UK had to release guidance on coping with noise annoyance, demonstrating the distress this noise signified. Another study conducted in London found that survey respondents perceived a decrease in outside noise but an increase in noise from neighbors, with noise annoyance rates increasing. In New York City during March 2020, the 311 System recorded a 42% increase in loud television complaints compared to the previous year. Overall, it was clear that while environmental and traffic noise level evaluation and annoyance significantly decreased during the lockdown, annoyance due to residential noise increased.

Past studies have demonstrated that noise annoyance during the COVID-19 pandemic was positively correlated with stress and anxiety levels. When linked to past findings that housing and demographic factors played a more significant role in noise complaints than road and rail noise, an interesting point is raised concerning noise complaints across neighborhoods and demographics throughout the COVID-19 pandemic.

**Current Reading**

- https://academic.oup.com/jpubhealth/article/42/3/448/5857760
- https://academic.oup.com/socpro/advance-article/doi/10.1093/socpro/spab075/6479622
- https://link.springer.com/article/10.1007/s10900-021-01006-y
- https://journals.sagepub.com/doi/pdf/10.1177/1078087416673202
- https://www.degruyter.com/document/doi/10.1515/noise-2021-0008/html
- https://www.sciencedirect.com/science/article/pii/S0048969721022841
- https://www.sciencedirect.com/science/article/pii/S0013935121015553
- https://www.sciencedirect.com/science/article/pii/S2210670721000603
- https://asa.scitation.org/doi/full/10.1121/10.0002667

### Setting Up 311 Data

In addition to conducting background research on 311 calls and noise complaints, I also downloaded and filtered the 311 Dataset. The original dataset from [NYC Open Data](https://nycopendata.socrata.com/Social-Services/311-Service-Requests-from-2010-to-Present/erm2-nwe9) is approximately 18GB, so I filtered the original dataset by date (2/13/2018 - 2/13/2023) and type of complaint (containing the word "Noise"). After these 3 million + rows finished downloading, I loaded them into an R dataframe. 

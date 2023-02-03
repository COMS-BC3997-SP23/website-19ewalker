---
layout: page
title: Project Proposal
permalink: /proposal/
---

## Project Proposal

For my project in COMS BC 3997, I plan to build a database-backed website that allows users to easily search data on violations and service requests at NYCHA developments.

### Why is this important?
Conditions in NYC housing projects have been [deteriorating over the past couple of decades](https://www.nytimes.com/interactive/2018/06/25/nyregion/new-york-city-public-housing-history.html) due to years of disinvestment of billions of dollars across all levels of government. In the early 2000s, the combination of this mass divestment in public housing and the rising costs to renovate and maintain buildings caused living conditions to take a turn for the worse, starting a cycle of cover-ups and a huge backlog of service requests. These conditions are reaching a fever pitch right now, with the NYCHA having [680K+ open work orders](https://eapps.nycha.info/NychaMetrics/Charts/PublicHousingChartsTabs/?section=public_housing&tab=tab_repairs)—their manageable workload is 90K open work orders. This backlog has real consequences for residents of NYCHA developments—not having hot water for days or weeks, waiting months for repairs, and walking up 50 flights of stairs per trip when the elevator is broken.

### Goals and Objectives

My goal is to create a centralized site in order to easily find all emergency food resources anytime, anywhere across all five boroughs.  I plan to first design an SQL database for all emergency food centers and then use online resources to populate this database with entries. After populating the database, I plan to create a database-backed website using Python and Flask in order to query the database. Finally, I will develop an intuitive user interface using HTML, CSS, and JS in order to finish the site. 

I would ideally like my final site to have a map page where people can see all available emergency food resources, and a main search page to find resources near you or near a given address. I want this search page to allow people to filter by days of the week and times of day available, faith, dietary restrictions, etc. Finally, this search page should include a filter allow users to see what is currently open.

### Method
**Timeline**
* Week of January 30th: Research existing solutions and resources
* Week of February 6th: Design SQL database
* Weeks of February 13th and 20th: Populate SQL database with real data
* Week of February 27th: Create site and connect to SQL database
* Week of March 6th and 13th: Get search page working for nearby food resources when you enter an address 
* Week of March 20th: Add search filters for dietary restrictions, times open, now open, etc
* Week of March 27th: Improve UX + design of search page
* Week of April 3rd and 10th: Create map page and get SQL entries to appear on it
* Week of April 17th: Add filtering to map page
* Week of April 24th: Improve UX + design of map page
* Week of May 1st: Wrap up and touch up design of site

Note: this is my general timeline, I left myself a buffer of time at the end in case this goes slower than I thought it would.

**Budget** 

I might need some money for compute credits depending on how I need to set up the PostGreSQL database. This is the only expense I forsee possibly having.

**Resources**

Food Pantries, Soup Kitchens, Food Banks, and Community Fridges lists
* [Food Help NYC](https://foodhelp.nyc.gov/locations)
* [FoodPantries.org](https://www.foodpantries.org/ci/ny-new_york)
* [Food Bank NYC](https://www.foodbanknyc.org/get-help/)
* [NYC Community Fridges](https://nycfridge.com/)
* [Free Meals in Manhattan](https://www.nyc.gov/html/mancb7/downloads/pdf/UWS%20free%20meals.pdf)


### Past Examples

I've worked on a couple projects in the past that used this combo of a Python/Flask backend and HTML/CSS/JS front-end in classes like COMS 4111: Databases COMS 4170: UI Design, and in my personal projects.  In COMS 4111, I also had the experience of designing an SQL database with a partner and attaching it to this Flask backend, allowing users to query our website. You can see a couple of these examples on [my website](http://www.elizabethwalker.site/coding). My internship last summer also prepared me for the hours of menial data entry the database population section of this project will entail.

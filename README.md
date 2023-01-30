# Find Food NYC
## Project Proposal

For my project in COMS BC 3997, I plan to build a database-backed website that provides up-to-date, accessible information on food pantries, soup kitchens, food banks, and community fridges open in New York City.

### Why is this important?
Food insecurity is reaching historic highs in New York City with a 69% increase in visits to food pantries and soup kitchens from 2019 to 2022 according to [City Harvest](https://www.cityharvest.org/food-insecurity/). Currently, 1.5 million New Yorkers are experiencing food insecurity, including 1 in 4 children. Within communities of immigrants and ethnic minorities, levels of food security are especially high with [31% of immigrants living in food-insecure households](https://aspe.hhs.gov/reports/how-are-immigrants-faring-after-welfare-reform). Community food pantries directly serve local residents facing food insecurity, and they are often one of the only sources of nutritious food in a neighborhood. They support low-income families, the homeless, and other vulnerable populations by promoting health and wellbeing. Food pantries can also provide additional resources like health screenings, back to school supplies, baby formula, and more. 

Despite the benefits and importance of these resources, there are still barriers to access for these resources. For instance, pantry hours are often extremely limited with one study showing that [53% of food pantries in the Bronx were open 3 hours per week or less] (https://link.springer.com/article/10.1007/s11524-012-9750-2). In this same study, listed hours and location on the Food Bank website were incorrect almost half of the time. Additionally, there is currently no user-friendly, centralized site to find all of the food pantries, soup kitchens, food banks, and community fridges. These resources are scattered across the website in lists, PDFs, and maps with no one source providing all of these tools. This lack of organization creates additional undue stress for those seeking resources.

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
* Week of March 20th: Add search filters for dietary restrictions, times open, etc
* Week of March 27th: 

**Budget** 

I might need some money for compute credits depending on how I set up the PostGreSQL database. This is the only expense I forsee possibly having.

**Resources**



### Past Examples

I've worked on a couple projects in the past that used this combo of a Python/Flask backend and HTML/CSS/JS front-end in classes like COMS 4111: Databases COMS 4170: UI Design, and in my personal projects.  In COMS 4111, I also had the experience of designing an SQL database with a partner and attaching it to this Flask backend, allowing users to query our website. You can see a couple of these examples on [my website](elizabethwalker.site/coding). My internship last summer also prepared me for the hours of menial data entry the database population section of this project will entail.

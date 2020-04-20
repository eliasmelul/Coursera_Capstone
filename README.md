# Coursera Capstone
<a href='https://nbviewer.jupyter.org/github/eliasmelul/Coursera_Capstone/blob/master/Capstone%20Project%20Final.ipynb'>View Notebook with Images</a>

This is the repository for the IBM Data Science Professional Certificate Capstone.

# Business Understanding and Business Problem

Have you every wondered if you should move to a place for a specific job? Whether you’d be happy in a place if you were to move?

The USA has over nineteen-thousand cities, towns and villages. About 310 of them are considered at least medium size with populations above 100,000. It’s easy to be overwhelmed when deciding to move, but it is especially true when you’re not sure what to expect from the place you might be moving to. 

Most people know in some way or another a city like New York, Boston, San Francisco, Chicago or Miami, but are otherwise unaware of the multitude of incredible cities in the US where they may be happier. People may be considering taking a job in a town they know little about, without knowing how similar it is to the cities they know they like or dissimilar from cities they know they dislike.

As an example, I love Boston and really like New York. I also really like Raleigh and Durham in North Carolina, but had I not attended Duke University, I would have not known. So now that I am graduating and considering job offers… where should I consider taking job in based on my preferences?

Our objective of this project is just that: clustering cities based on an amalgam of features and creating a recommendation system that, based on my input (or yours!), recommends cities based on these clusters and the city profiles of your rated cities.

# Data Requirements and Collection

To properly segment cities in the USA and create a competent recommender system, I need to generate detailed city profiles for each city in the study. This begs the following questions:

**Which cities will I include?**

The Wikipedia site ‘List of United States cities by population’ deemed appropriate for these purposes. Ideally, we would try to include a lot more cities, but the computational requirements to use thousands of cities instead of the largest 315 by population seems too high for the marginal benefit. 

**What data will be collected and how?**

There is an enormous amount of data available on the web regarding cities, but a lot of it comes from untrustworthy sources, nor is it standardized. Lucky me, I found datausa.io, from which I can scrape a lot of relevant information from each city and generate good city profiles (Thank you Deloitte and Datawheel!). I will selectively scrape some metrics that I believe are important and combine them with information about the categories of the top 100 venues in each city from Foursquare’s API to complete the city profiles.

**Some of the metrics scraped and included are:**

*Population and Population Change (Year to Year)
*Poverty Rate
*Median Age
*Median Household Income and Median Household Income Change (Year to Year)
*Number of Employees and Number of Employees Change (Year to Year)
*Median Property Value and Median Property Value Change (Year to Year)
*Average Male and Female Salary, and a ratio of Average Male to Female Salary
*Gini coefficient in 2017 and 2018, as well as it's change (Year to Year)
*Ratio of Patients to Clinicians (county-wise)
*Foreign-born population percentage
*Citizen population percentage
*Total degrees awarded in 2018 (higher education)
*Male to Female ratio of awarded degrees
*Number of degrees per capita
*Number of households in city
*Population per household (people per household)
*Homeownership Percentage (Rent vs Own)
*Average Commute Time (minutes)

**To see the final dataset, <a href='https://github.com/eliasmelul/Coursera_Capstone/blob/master/cities_profiles_freqVenues.csv'>click here</a>**

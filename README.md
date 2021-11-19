# Coursera_Capstone_Final_Project
Introduction: Business Problem
In this project we will try to find an optimal location for a restaurant. Specifically, this report will be targeted to stakeholders interested in opening an Turkish restaurant in Tashkent, Uzbekistan.

Since there are lots of restaurants in Tashkent we will try to detect locations that are not already crowded with restaurants. We are also particularly interested in areas with no Turkish restaurants in vicinity. We would also prefer locations as close to city center as possible, assuming that first two conditions are met.

We will use our data science powers to generate a few most promissing neighborhoods based on this criteria. Advantages of each area will then be clearly expressed so that best possible final location can be chosen by stakeholders.

Data
Based on definition of our problem, factors that will influence our decission are:

- number of existing restaurants in the neighborhood (any type of restaurant)
- number of and distance to Turkish restaurants in the neighborhood, if any
- distance of neighborhood from city center
We decided to use regularly spaced grid of locations, centered around city center, to define our neighborhoods.

Following data sources will be needed to extract/generate the required information:

- centers of candidate areas will be generated algorithmically and approximate addresses of centers of those areas will be obtained using Google Maps API reverse geocoding
- number of restaurants and their type and location in every neighborhood will be obtained using Foursquare API
- coordinate of Tashkent center will be obtained using Google Maps API geocoding of well known Tashkent location

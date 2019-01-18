# Coursera_Capstone
Repository for the  Coursera:Applied Data Science Capstone

# Introduction/Business Problem

Our client would like to open a pub in Budapest. The goal for the project is to find the best place for a new pub. It is crucial to find the right location for businesses, most of the time it is the deciding factor in the beginning of the business.
This information can be useful for anyone who wants to open a bar or a pub in the city.
I will use the Foursquare API to solve the problem. To find the best place it`s important to find the already existing places, which places are popular and if is there any room for a new business.
There are also regulations where you can open a pub, in our case it has to be at least 150 meters from any public school.

# Data

I will use the disticts of Budapest and parse all the coordinates from pages.
This page can be used to parse the GPS coordinates for all districts in Budapest: http://nepesseg.com/budapest/budapest-01-kerulet
Based on the GPS coordinates the Foursquare API can be used to get all the necessary information. Based on the Foursquare API I will filter out the similar businesses and get the most popular districts. The API can also help to find out businesses or landmarks, which helps to attract more visitors. 
For the law regulation, I will also use the public school information, with street data and convert them to gps coordinate to parse the exact location for them.

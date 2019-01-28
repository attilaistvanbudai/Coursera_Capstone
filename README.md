# Coursera_Capstone
Repository for the  Coursera:Applied Data Science Capstone

# Introduction/Business Problem

Our client would like to open a pub in Budapest. The goal for the project is to find the best place for a new pub. It is crucial to find the right location for businesses, most of the time it is the deciding factor in the beginning of the business.

This information can be useful for anyone who wants to open a bar or a pub in the city.

I will use the Foursquare API to solve the problem. To find the best place it`s important to find the already existing places, which places are popular and if is there any room for a new business.

There are also regulations where you can open a pub, in our case it has to be at least 150 meters from any public school.

# Data

I will use the districts of Budapest and parse all the coordinates from pages.

This page can be used to parse the GPS coordinates for all districts in Budapest: http://nepesseg.com/budapest/budapest-01-kerulet
Based on the GPS coordinates the Foursquare API can be used to get all the necessary information. Based on the Foursquare API I will filter out the similar businesses and get the most popular districts. The API can also help to find out businesses or landmarks, which helps to attract more visitors. 

For the law regulation, I will also use the public school information, with street data and convert them to GPS coordinate to parse the exact location for them.

# Methodology

I tried to concentrate on the interesting locations, so I filtered the most popular districts. Due to the limited number of premium calls per day, I used get details about the pubs from the five most popular districts.

The most popular districts are: 1st,5th,6th,7th,8th

I needed to have some preprocessing for the data, and fill in empty dataset.

I used linear regression to find out which attributes are modifying the ratings and the number of likes. I also analyzed the neighborhood for each location to find out what kind of venues affect positively or negatively the number of likes.

# Results

The results can be seen in the notebook. In summary:
PriceRate/Credit card payment/Reservations affect positively the rating
Dinner/Lunch or Happy hours are negative for the final ratings

The ideal neighborhood contains: some restaurants/bars/cafe
The venues affect the location negatively: Other pub, Beer Store, Supermarket, Pharmacy

I have created a heatmap which shows the ideal location by green and the bad location with red. It also contains the school locations.

# Discussion

Based on the existing data, there are some nice places in the inner city. Based on my knowledge they are the most expensive part of the city, so we might need to have further exploration and weighting the location by price.

# Conclusion

The Foursquare API is not really popular in Budapest, however it can be used to extract some meaningful information about the venues. However they might not be statistically relevant, because the sheer number of data is not enough. 


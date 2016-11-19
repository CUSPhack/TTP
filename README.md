# TTP
taxi tipping in NYC

Github username of Collaborators:
poonehfamili
lx565
streich676

Problem Description: Questions:
Where are the highest cab tips occurring in NYC? 
Does location matter for the amount people tip cab drivers? Once we discover the areas in which cab drivers are better compensated we may be able to infer what are the main variables for tipping. Does the age of the rider matter? Do those who live in more expensive neighborhoods tip cab drivers better. 
Data: We acquired a nice cleaned dataset online from a data enthusiast, Todd W Schneider,  who cleaned the data for his own means. The taxi data includes lat/long of origin and destination, tip amount and total fare. This data can be found here:
https://github.com/toddwschneider/nyc-taxi-data/blob/master/raw_data_urls.txt
In order to project the data geospatially we used a shapefile obtained from NYC.gov.  This shapefile is of NYC, all boroughs included, and includes lat long coordinates of NYC census tracts. 
NYC.policymap.com mean age by Census Tract. 
Analysis: To discern if there was a difference in tip amount by destination location we calculated the tip as a percentage of the total fare. We then grouped the destinations into their respective Census blocks. Following this we took the mean of the tip percentages grouped by Census tract. We found the mean of the the tip percentage as 19.70%. The standard deviation of the tip percentage was 9.84. 



Deliverable: We wish to create a static map which displays the mean tip amount for taxi rides which end in a certain census tract. Once this is complete we would like to create the same map but based on the taxi rides origin. 
Conclusions: We now have the infrastructure in place in order to scale up our analysis. From our initial analysis of 10,000 trips the mean is 19.70%.  Our standard deviation is 9.84%. From our map you can see that there is not much deviation from 20% based on location. Notable exceptions are JFK airport. Our initial analysis also suggests that the distribution of tips is normal.   


Tools: Matplotlib
	Pylab 
	Geopandas
	Shapely







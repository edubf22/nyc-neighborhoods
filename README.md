# Clustering NYC Neighborhoods
<p style="text-align: center;"><b> Midterm project - LHL Data Science Bootcamp </b></p>

![New York City](/output/figures/emiliano-bar-kheTI8pIywU-unsplash.jpg)
_Figure credit: [Emiliano Bar](https://unsplash.com/photos/kheTI8pIywU?utm_source=unsplash&utm_medium=referral&utm_content=creditShareLink)_

## Introduction
In this project, we aimed to segment neighborhoods in New York City (NYC) into different clusters based on the availability of healthcare services. 

Clustering was done using different models from the Scikit-Learn package, such as the K-means algorithm, hierarchichal clustering and DBScans. Venue information was obtained using the Foursquare API.

        Add information on the new data file? 
        Add a summary of our findings? 

The ```notebooks``` folder contains the code used during the data processing, modelling and figure generation steps. The resulting .csv file containing the neighborhoods and respective cluster labels can be found in the ```output``` folder, as well as the figures generated during the data visualization step.   

## Data acquisition
Geolocation on each NYC neighborhood was obtained from the nyc_geo.json file. After acquiring the coordinates for each neighborhood, we sent GET requests to the Foursquare API to get venue information within a 500 m radius for each neighborhood. 

Economic information relates to the median house pricing for different neighborhoods in NYC. Some of the median prices had to be estimated since there was missing information for 1-Bedroom and Studio apartments.
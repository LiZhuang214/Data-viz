---
title: "AirBnB Listings in Barcelona, Spain"
date: 2019-05-11
published: true
tags: [dataviz, folium, hvplot, altair]
excerpt: "Embedding interactive Folium charts on static pages using Jekyll."

altair-loader:
  altair-chart-1: ["charts/alt_chart.json"]
  altair-chart-2: ["charts/listing_price.json"]
  altair-chart-3: ["charts/listing_polarity.json"]
  altair-chart-4: ["charts/Sentiment_alt.json"]

hv-loader:
  holoviews-chart-1: "charts/hvheatmap_1.html"
  holoviews-chart-2: "charts/hvheatmap_2.html"
  holoviews-chart-3: "charts/hvheatmap_3.html"
  

folium-loader:
  folium-chart: ["charts/Barcelona_heatmapstest.html", "400"]
toc: true
toc_sticky: true
---

## Project Overview
   The project will explore the Airbnb market in Barcelona, Spain using data from [Inside Airbnb](http://insideairbnb.com/get-the-data.html). I will explore the spatial distribution of Airbnb prices and its relation to the district in which the unit located. Districts’ information includes but not limited to the concentration of restaurants, tourist attractions, and other accommodation options. The landmarks and restaurants data can be obtained from [tour-pedia.org API](http://tour-pedia.org/api/index.html). 

## Folium Layers Map
   You can turn on and off different layers to discover the airbnb listings, tourists attractions and restaurants here.
Click on the camera icon to get more information about this tourist place!

<div id="folium-chart"></div>

   From the layer of Airbnb listings Density, the lower heart area of Barcelona, which consists of neighborhoods centered with la Dreta de i’Example, has the largest density of Airbnb housings. In specific, according to the layer of Airbnb listings in Barcelona, the neighborhoods around the lower east coast contributes the most Airbnb facilities; at the same time, the western areas are with very few Airbnb housings. The restaurant density generally follows the trend of Airbnb density, which gathered around the lower heart area of the city, while in the neighborhoods of most west corner it also indicates a high density of restaurants.
   Combining the layers of Tourists Attractions and Attractions density, it is interesting to discover that the lower heart area is with most attractions while in general the attractions are more scattered around in the city, compared with the trends of Airbnb and restaurants. 


## Altair Charts
_Average airbnb price per person at different neighbourhoods._ 
<div id="altair-chart-2"></div>

   From Airbnb listing Price Choropleth Map, the four neighborhoods located at the center, east and east coast leading the average listing price, where la Vila Olimpica del Poblenou with the highest average listing price/person of 184 Euros. Generally, the south part of the city is with higher average listing price/person than that of the north part of Barcelona.

_Average overall satisfaction on airbnb listing at different neighbourhoods._
<div id="altair-chart-3"></div>

   At the meantime, according to Airbnb listing Satisfaction Chloropleth Map, Baro de Viver, el Turo de la Peira and Vallvidrera, el Tibidabo i les Planes, the three neighborhoods of north Barcelona, are ranked top with the Average Satisfaction index. However, for the rest parts of the city, it is indicated that the Average satisfaction index grows from north of the city to the coast, south area. 
   In all, as the pricing and satisfaction elements combined from the two Chloropleth Map, it can be defined that the Airbnb facilities at the west, and also the south coast area, are advantageous both for their price and quality.
  
## Hvplots

<div id="holoviews-chart-1"></div>

   According to the first plot, it is predictable that the overall price for shared room is cheapest; the private room is in the middle; and that for the entire home/apt is most expensive. From another perspective, the price difference for different areas in the city, in speaking of shared room and private room, is not obvious. Nevertheless, there are big price gaps among the entire home/apt type in different areas. For instance, the price for entire facility in la Font d’en Fargues is claimed about 430 Euros per person per night, whereas for Baro de Viver that is only 25 Euros. 

<div id="holoviews-chart-2"></div>

   The second graph indicates that a satisfaction level between 0.2-0.3 is dominant for the all three mentioned types of Airbnb housings, where the entire home/apt and private room are with relatively higher satisfaction level. The shared room type contributes most level 0 type; the private room type contributes no 0-level satisfaction, and the best rated one is the private room at Baro de Viver.

<div id="holoviews-chart-3"></div>

   From the last graph, the two super-strict types and the strict types are with limited data, and for the other tree types at the left half of the graph, the satisfaction level for the moderate type is slightly better than the rest of two.

## Cluster Analysis

<div id="altair-chart-4"></div>

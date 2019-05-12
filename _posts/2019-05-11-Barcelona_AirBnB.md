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

This post will show examples of embedding interactive maps produced using [Folium](https://github.com/python-visualization/folium).
## Project Overview
  The project will explore the Airbnb market in Barcelona, Spain using data from [Inside Airbnb](http://insideairbnb.com/get-the-data.html). I will explore the spatial distribution of Airbnb prices and its relation to the district in which the unit located. Districts’ information includes but not limited to the concentration of restaurants, tourist attractions, and other accommodation options. The landmarks and restaurants data can be obtained from [tour-pedia.org API](http://tour-pedia.org/api/index.html). 

## Folium Layers Map

<div id="folium-chart"></div>

You can turn on and off different layers to discover the airbnb listings, tourists attractions and restaurants here.
Click on the camera icon to get more information about this tourist place!

## Altair Charts
Average airbnb price per person at different neighbourhoods. 
<div id="altair-chart-2"></div>

Average overall satisfaction on airbnb listing at different neighbourhoods.
<div id="altair-chart-3"></div>


## Hvplots

<div id="holoviews-chart-1"></div>

<div id="holoviews-chart-2"></div>

<div id="holoviews-chart-3"></div>

## Cluster Analysis

<div id="altair-chart-4"></div>

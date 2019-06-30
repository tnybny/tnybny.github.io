---
title: 'Conditional probability maps of extreme temperatures'
date: 2016-01-01
permalink: /posts/2016/01/Conditional-probability-maps/
tags:
  - R Shiny
  - Extreme event detection
---

So I created my first [R Shiny](https://shiny.rstudio.com/) app and I obviously think its pretty cool. Props to the Shiny team for making the learning process of how to make these apps so enjoyable.

Basically for the North American region, you can specify a location and get back a spatial conditional probability map with that location as a reference. To put it in concrete terms, you'll get back the probability of there being extreme values in other locations given there was an extreme value in the reference location. Its pretty cool to observe the land vs. sea differences and the east coast vs. west coast.

##Some interesting observations are:
* Locations close to the reference location having a higher conditional probabilities compared to locations further away (autocorrelation in space).
* Cold extremes tend to have higher extent of influence.
* The extent of influence of an extreme in the sea is generally broader compared to those on land.
* Events that occur on the east cost of the US are usually oriented along the coastline and are ellipse shaped.

You can find the app [here](https://tnybny.shinyapps.io/Spatial_conditional_probability_maps/) and the source code [here](https://github.com/tnybny/Spatial-conditional-probability-maps)

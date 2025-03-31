---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: 'Assignment 2: The San Fransisco crime crawl – Where Data Meets Drama!'
---

# Suspect: The Dataset
In this one-pager, we explore distinct temporal patterns in crimes across San Francisco — focusing on Robbery, Assault, and Weapon Law crimes. What if the timing of these crimes could tell us more than the crimes themselves?
To support this exploration, the dataset used in this analysis consists of reported crime incidents in San Fransisco from 2003 till present and is sourced from the [San Fransisco Police Department Incident Reports](https://data.sfgov.org/browse?category=Public+Safety&sortBy=relevance&page=1&pageSize=20). The data was accessed on June 2, 2025, which serves as the cutoff date. To ensure consistency and complete annual coverage, we focus exclusively on data from 2003 to 2024.  

# Are These Crimes Partners in Crime?

The figure below presents three scatter plots showing the temporal relationships between Robbery, Assault, and Weapon Law crimes over the 168 hours of a standard week (7 days × 24 hours). Each point represents one hour during the week (for example, hour 150 is Sunday morning at 6 AM, shown as dark purple gradient). Therefore, each panel contains 168 scatterpoints, where the placement of the scatterpoint is determined by the count of crime 1 (x-axis) and the count of crime 2 (y-axis) during that hour. This provides a visual comparison of how these crime types vary and potentially align over the hours of the week.
<!-- Calendar Figure -->
<div style="text-align: center;">
  <img src="Calender.png" width="150%" />
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 2: The subplots show fairly correlated data between the crime categories Robbery, Assault and Weapon Law. Each scatterpoint represents an hour during the week (0-168) with a total of 168 scatterpoints in each subplot.
  </p>
</div>
The fairly strong positive correlations suggest these crimes often co-occur, potentially driven by shared social or environmental circumstances. The displayed R&sup2; values indicates positive correlation, meaning that when one type of crime increases, the second tends to increase too, and vice versa. Notably, crime intensity builds toward the weekend, indicating more incidents of assault, robbery and weapon law related crimes reported as the city’s tempo rises.

This visualization supports the assumption that the three crime categories are sufficiently correlated to be treated as a single combined category. However, even on weekends, there are quieter moments — likely in the early mornings — though these are harder to spot due to the limits of the color gradient. In the next visualization, we’ll use this grouping to further uncover how crime pulses through the rhythm of the week.


# When Does the City Get Sketchy?
<div style="text-align: center;">
  <iframe src="my_bokeh_plot.html" width="150%" height="420" frameborder="0"></iframe>
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 1: The most likely times of the day throughout the week to find your drunk friend in San Francisco based on aggregated event data. Further, one can interactivelt choose specific time intervals.
  </p>
</div>

# Which SF District Turns Into a Crime Scene After Dark?
So you want to stay safe from crimes and potentially getting your wallet robbed in San Fransisco? Best to stay at home! No don't worry, we have constructed a dynamic heatmap throughout the years (2003-2024) that shows where most of the reported incidents for these crimetypes occur in San Fransisco. Due to the insights from the previous visualization, the heatmap only considers weekend nights (Friday and Saturday) between 8 PM and 4 AM. 
<!-- Interactive Crime Map Figure -->
<div style="text-align: center; margin-top: 30px;">
  <iframe 
    src="crime_map_weekend.html"
    width="100%" 
    height="800px" 
    frameborder="0"
  ></iframe>
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 3: Distribution of aggregated Assault, Robbery, and Weapon law incidents occurring on Friday and Saturday nights (8 PM - 4 AM) in San Francisco, based on reported data from 2003 to 2024.
  </p>
</div>
So what does the heatmap show us? If you are willing to take the risk, the vibrant districts Mission and Southern is home to [dense nightlife and vibrant bars](https://sanfranciscodrinksguide.com/en/blog/where-to-drink-93/bars-98/bar-hopping-in-the-mission-district-90.htm), however also home to consistently the highest counts of assaults, robberies and weapon law crimes throughout the years. Meanwhile, Richmond and Sunset districts sleep soundly under a blanket of low crime, their suburban calm rarely disturbed and known for a (family friendly environment)[https://sanfranciscodrinksguide.com/en/blog/where-to-drink-93/bars-98/bar-hopping-in-the-mission-district-90.htm]





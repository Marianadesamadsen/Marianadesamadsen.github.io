---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: 'Assignment 2: The San Fransisco crime crawl – Where Data Meets Drama?'
---

# Data Description:

The dataset, sourced from the San Francisco Police Department Incident Reports, includes reported incidents spanning from 2003 to the present. For this analysis, the data was accessed on June 2, 2025, which serves as the cutoff date. To ensure consistency and complete annual coverage, we focus exclusively on data from 2003 to 2024. Our study centers on three key crime categories: Robbery, Assault, and Weapon Law Violations, which will be known to be highly correlated.

# Are These Crimes Partners in Crime?

The figure below presents three scatter plots showing the temporal relationships between Robbery, Assault, and Weapon Law Violations over the 168 hours of a standard week (7 days × 24 hours). Each point represents the number of reported incidents during a specific hour, providing a visual comparison of how these crime types vary—and potentially align—over the hours of the week.
<!-- Calendar Figure -->
<div style="text-align: center;">
  <img src="Calender.png" width="150%" />
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 2: The subplots show highly correlated data. Each data set are temporal .
  </p>
</div>
There is a strong correlation between all the selected crime types. The $R^2$ values indicates positive correlation, meaning  


supporting the assumption that they can be reasonably combined into a single category. 


# When Does the City Get Sketchy?
<div style="text-align: center;">
  <iframe src="my_bokeh_plot.html" width="150%" height="420" frameborder="0"></iframe>
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 1: The most likely times of the day throughout the week to find your drunk friend in San Francisco based on aggregated event data. Further, one can interactivelt choose specific time intervals.
  </p>
</div>

# Which SF District Turns Into a Crime Scene After Dark?
<!-- Crime Map Figure -->
<div style="text-align: center; margin-top: 30px;">
  <img src="crime_map.png" width="150%" />
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 3: Distribution of normalized assault, robbery, and weapon law incidents occurring on friday and saturday nights in San Francisco, based on reported data from 2003 to 2024.
  </p>
</div>
We notice on the map of the crime data distribution that most of the reported arrests for our focused crime types happens in the southern district.





---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
title: 'Assignment 2: The San Fransisco crime crawl – Where Data Meets Drama?'
---

Data Description:
San Francisco [Police Department Incident Reports](https://data.sfgov.org/browse?category=Public+Safety&sortBy=relevance&page=1&pageSize=20), covering incidents from 2003 to present. The data was loaded on **06/02/2025**, making this the cutoff date. However, we have only used data from **2003–2024** to ensure full-year coverage. 

What day of the week will you find your drunk friend in San Fransico? 
<div style="text-align: center;">
  <iframe src="my_bokeh_plot.html" width="150%" height="420" frameborder="0"></iframe>
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 1: The most likely times of the day throughout the week to find your drunk friend in San Francisco based on aggregated event data. Further, one can interactivelt choose specific time intervals.
  </p>
</div>

What days of the year will your friend be drunk in San Fransico? 
<!-- Calendar Figure -->
<div style="text-align: center;">
  <img src="Calender.png" width="150%" />
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 2: Estimated days your friend will be drunk in San Francisco based on calendar patterns.
  </p>
</div>


What district in San Fransico will you find your lost drunk friend in San Fransico?
<!-- Crime Map Figure -->
<div style="text-align: center; margin-top: 30px;">
  <img src="crime_map.png" width="150%" />
  <p style="font-style: italic; font-size: 0.9em; color: gray;">
    Figure 3: Normalization of arrests in districts of San Francisco, based on crime density.
  </p>
</div>
We notice here that the southern district has the biggest density of arrests for drunkeness. Even though most of the bars in san fransico are placed in the central district, the southern district still shines in terms of arrests for drunkeness.





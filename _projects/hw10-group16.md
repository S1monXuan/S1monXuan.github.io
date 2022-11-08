---
name: Homework10-Group16
tools: [Python, vega-lite, altair]
image: assets/pngs/temperature.png
description: Homework 10 Group 16 Data Visualization
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Homework10-group16

Group Member: Xinmai Xuan, Peng Lu, Xiao Zhang
# PLOT 1

1. Description of the visualization:
    In the first plot, we use the `Big Foot` dataset to show the range of highest temperature in each states people obeserved big foot.
2.  Design choices: 
    + Axis: we set x-axis to show the temperature range and y-axis to show the states.
    + Encoding: `temperature_high` is quantitative, and `state` is ordinal instead of nomial because we want it to be automatically sorted by alphabetical.
    + Color scheme: We use greenblue color scheme.
3. Data transformations: we divided the `temperature_high` into bins.
4. Improvement from HW9: we don't use hw9 from anyone in our group.

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10_pt1.json" style="width: 100%"></vegachart>

# PLOT 2

1. Description of the visualization:
    In the second plot, we show the recurrence of precipitation probability in the places people obeserved big foot.
2.  Design choices: 
    + Axis: x-axis is the range of precipitation probability and y-axis is the frequency.
    + Encoding: `precip-pobability` is quantitative, and `recurrence` is ordinal, a discrete ordered quantity by calculation.
    + Color scheme: We use defult color.
3. Data transformations: we divided the `precip-pobability` into bins, grouped the data by the bins, and count the number for in each bin.
4. Improvement from HW9: we don't use hw9 from anyone in our group.

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10_pt2.json" style="width: 100%"></vegachart>


# Interaction

**Specify what interactivity you chose for one (or more) plots and how this helps your visualization be more clear or interesting:**

We first plotted a grid-heat map between each state and its high temperature in the places people observed big foot, and then created a bar chart of the recurrence of precip-probability. Through interactivity, we can explore the recurrence of precipitation probability for specific State at different temperature range intervals. What interesting we find is in the places has higher temperature, the recurrence of precipitation is higher too.

<vegachart schema-url="{{ site.baseurl }}/assets/json/hw10_fi.json" style="width: 100%"></vegachart>

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_bcubcg_fall2022/main/data/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/S1monXuan/S1monXuan.github.io/blob/main/assets/notebook/homework10-group16.ipynb" text="The Source Code" %}
</div>


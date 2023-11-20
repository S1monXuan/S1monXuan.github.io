---
name: IS445 FinalProject Group25
tools: [Python, vega-lite, altair, geopandas, myblinder]
image: assets/pngs/fin25-EU-map.png
description: Homework 10 Group 16 Data Visualization
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Final Project - group25

Group Member: Xinmai Xuan, Peng Lu, Xiao Zhang

# Introduction

The greenhouse effect is currently the most important problem that the world wants to solve, and forests are considered to be the most important factor in solving this problem. Therefore, we want to analyze and visualize the Gross increase and Use intensity of forests to analyze the role of forests in the greenhouse effect and to draw conclusions. In addition, we also include the gases that affect the greenhouse effect in the reference range, so that we can have more evidence for our conclusions. In our group project, we mainly use ten countries in Europe as the sample for the analysis, and we hope to draw conclusions about the effect of forests on the greenhouse effect.

# Figure 1

We create a visualization (Figure 1) showing the annual forest Gross increase and its Use intensity for these European cities. We first create a grid heat map between year and Gross increase, which shows the forest growth in terms of color shades. Then, we create a histogram with the Use intensity (median) of the forest for each year and link it to the heat map. By selecting the grid in the heat map, we can get the average forest usage rate per year in the histogram. The more you select the grid, the more you can get the gross increase and the average use of the forest in different years. From this analysis, we can see that although some cities do not have very high gross forest increase, the average forest usage rate is very high. Also, for those areas with high gross increase, the forest usage rate is higher than for those areas with low growth rates.

<vegachart schema-url="{{ site.baseurl }}/assets/json/fin25_dashboard.json" style="width: 100%"></vegachart>

# Figure 2

To explore more information about the relation between forest-resource usage and green-gas emissions. We purpose a new dashboard. The left side shows forest-resource usage data on a selected EU map. In the right plot, users could check the line chart based on the country name and selected green-gas type.

Unfortunately, we can not convert this dashboard to JSON since it needs a python kernel. We adopt myblinder, an online jupyter notebook solution to solve this problem. You can use this link [Dashboard2](https://mybinder.org/v2/gh/S1monXuan/is-445-finalproject-demo2/HEAD) to open a jupyter notebook online to use our dashboard. **It may take several minutes to open this notebook**

We also show figures separately in this post, please feel free to check those figures.

## EU map

**This is just a screen shot to display our map.** 

In Dashboard, you can check the value of Froest Resource in different years using a menu created by ipywidgets. By selecting different years, the map would display different layers.

<img src="{{ site.baseurl }}/assets/pngs/fin25-EU-map.png" alt="image"/>

## Line chart

The main factor affecting the greenhouse effect is carbon dioxide content, so we made a line chart of the carbon dioxide for each country. From the plot, we can see that Germany (DEU) has the most carbon dioxide emissions, which is consistent with the fact that Germany is a large industrial. And Denmark (DNK), Portugal (PRT), Austria (AUT) and Ireland (IRL) have consistently low CO2 emissions. As people pay more and more attention to ecology, we can see that overall, the carbon dioxide emissions of these countries have declined to a certain extent.

Source code of this line chart: [Source Code](https://raw.githubusercontent.com/S1monXuan/S1monXuan.github.io/main/assets/json/fin25-linechart.vl.json)

<vegachart schema-url="{{ site.baseurl }}/assets/json/fin25-linechart.vl.json" style="width: 100%"></vegachart>

<!-- these are written in a combo of html and liquid --> 

<div class="left">
{% include elements/button.html link="https://github.com/lovefade/lovefade.github.io" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/S1monXuan/S1monXuan.github.io/blob/main/assets/notebook/FinalProject-Group25.ipynb" text="The Source Code" %}
</div>


---
name: Homework 5
tools: [Python, HTML, vega-lite]
image: assets/json/chart1.png
description: This is my page for IS 445 Homework 5
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Chart Write-ups

Chart 1: I made a graph that shows the number of Bigfoot sightings per state. I decided to plot State on the X axis and Number of sightings on the Y axis. I used a bar chart to clearly show the levels of each state's sightings and make it easy to compare each value. I decided to keep the color scheme minimal for easy readability. Since there are 50 states, I thought that having each state be a different color would make the graph too busy, so I decided to keep everything in the default blue and clearly label my axes so that the user could understand the graph at first glance. I also made it a point to aggregate the total sighting counts by state so that they could be translated to a bar chart easily and clearly.

Chart 2: I made a graph that shows the number of Bigfoot sightings per season. I made this graph similarly to Chart 1, with clearly labeled axes, aggregated total sighting counts by season for easy translation, and a bar chart visualization so that the user would be able to compare each season's count to the others. For this chart, I included a dropdown that would highlight each season's bar in a different color while graying out all the other bars. This lets the user focus in on a specific season's count without having to worry about getting it mixed up with the others. Each season's bar also has a different color when selected, which helps the user further differentiate between bars. Overall, this interactivity would help a user who finds it difficult to trace a chart and zero in on a desired value or category.

<vegachart schema-url="/assets/json/chart2.json" style="width: 100%"></vegachart>

<vegachart schema-url="/znquraishi.github.io/assets/json/chart1.json" style="width: 100%"></vegachart>


# Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 

<div class = "left">
{% include elements/button.html link="https://raw.githubusercontent.com/UIUC-iSchool-DataViz/is445_data/main/bfro_reports_fall2022.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/znquraishi/znquraishi.github.io/blob/main/python_notebooks/Workbook.ipynb" text="The Analysis" %}
</div>


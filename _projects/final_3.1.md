---
name: Final Part 3.1
tools: [Python, HTML, vega-lite]
image: assets/json/chart1.png
description: This is my page for IS 445 Final Part 3
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---


# Paragraph 1

Group Member (solo): Zayna Quraishi

Title: What we learn from data on death
Author: Zayna Quraishi

From a public health perspective, it is very important to track data relating to the leading causes of death in the United States. This data exploration gives insight into the deadliest conditions in the U.S., the states most and least impacted by them, and overall health trends. In this article, we'll take a look at how the leading causes of death impact American states by mapping each state's age-adjusted death rate. An age-adjusted death rate, according to the Missouri Department of Health and Senior Services, is a way to measure death rates without extra factors that may impact an age group's overall health skewing the data.

First, we'll take a look at the states with the overall highest age-adjusted death rates. From the chart below, we see that Mississippi leads with a rate of around 160.

<vegachart schema-url="/assets/json/top10.json" style="width: 100%"></vegachart>

# Paragraph 2

Next, we'll take a look at the states with the overall lowest age-adjusted death rates. From the chart below, we see that Hawaii has the lowest of all the states, with a rate of just under 100.

<vegachart schema-url="/assets/json/bottom10.json" style="width: 100%"></vegachart>

# Paragraph 3

Overall, we can see the differences between the Top 10 and Bottom 10 states. For example, most of the states in the Top 10 are southern states, while most of the states in the Bottom 10 are located on either the East or West Coast. However, we can go even deeper into the data to pinpoint the causes behind each state's death rate. This is an important part of actionable data--by learning the top causes of death in a certain state, officials and experts can then make a plan to mitigate this risk.

Let's take a look at the top 5 causes of death for Mississippi, the state with the highest age-adjusted death rate:

<vegachart schema-url="/assets/json/miss.json" style="width: 100%"></vegachart>

# Paragraph 4

From the chart, we see that heart disease and cancer are the two highest causes of death in Mississippi. This process can be repeated with other states in the Top and Bottom 10 to identify the causes that are the most deadly for Americans and find ways to provide healthcare to affected residents.

Source (all visualizations are my own):
Missouri Department of Health and Senior Services. (n.d.). Age-adjusted death rates (AARate) documentation. https://health.mo.gov/data/mica/CDP_MICA/AARate.html




# Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 

<div class = "left">
{% include elements/button.html link="https://github.com/znquraishi.github.io/_data/NCHS_-_Leading_Causes_of_Death__United_States.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/znquraishi/znquraishi.github.io/blob/main/python_notebooks/Final3_Workbook.ipynb" text="Analysis and Code for All Visualizations" %}
</div>


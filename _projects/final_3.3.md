---
name: Final Part 3.3
tools: [Python, HTML, vega-lite]
image: assets/json/chart1.png
description: This is my page for IS 445 Final Part 3.3
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---



Group Member (solo): Zayna Quraishi

# Mississippi cancer trends and location
# By Zayna Quraishi

Public health research is essential to the overall health and wellbeing of the United States. By studying healthcare access, regional effects of diseases and conditions, and death rates, experts can make informed policy decisions that keep us all safe. In this article, we'll apply these studies to Mississippi. According to the contextual bar chart below, Mississippi has the highest age-adjusted death rate in the U.S.  This makes the state a priority for public health officials to examine in order to determine critical areas that are being affected by health conditions.

Hover over the bar chart below to see exact age-adjusted death rates for the 10 states with the highest rates. An age-adjusted death rate, according to the Missouri Department of Health and Senior Services, is a way to measure death rates without extra factors that may impact an age group's overall health skewing the data.

<vegachart schema-url="/assets/json/top10 (1).json" style="width: 100%"></vegachart>

According to the contextual bar chart below, which shows the top 5 causes of death in Mississippi, cancer is the second-deadliest condition in the state. Thus, it is worth it to explore how cancer affects the population to determine where public health policy should primarily go into effect.

Hover over the bar chart below to see exact age-adjusted death rates per cause of death.

<vegachart schema-url="/assets/json/missCauses.json" style="width: 100%"></vegachart>

The following scatter plot shows the distribution of cancer rates by county based on age-adjusted incidence rate and average annual count of cases. This gives insight into the actual impact of cancer on different communities. For example, a county that may have a lower annual count due to a smaller population could have a higher incidence rate, showing a high presence of the condition. The plot also shows the differences in rural and urban counties, giving insight into areas where cancer is more prevalent.

Hover over each point on the chart below to see exact statistics, county names, and rural/urban codes.

<vegachart schema-url="/assets/json/countyRates.json" style="width: 100%"></vegachart>

Overall, we see that cancer rates among urban counties remain more constant than those among rural counties, even as the average annual case count increases. Quitman County and Choctaw County, with the highest and lowest rates overall, respectively, are both rural. Based on this data, it may be prudent for public health research to center around rural counties in Mississippi in order to answer why cancer affects these communities in different ways, and why they hold more variance in rates than urban areas.

# Sources (all visualizations are my own):
Missouri Department of Health and Senior Services. (n.d.). Age-adjusted death rates (AARate) documentation. https://health.mo.gov/data/mica/CDP_MICA/AARate.html

Contextual Visualization Data: Centers for Disease Control and Prevention, National Center for Health Statistics. (2025). NCHS—leading causes of death: United States [Data set]. Data.gov. https://catalog.data.gov/dataset/nchs-leading-causes-of-death-united-states

Primary Visualization Data: National Cancer Institute. (n.d.). State cancer profiles: Incidence rates—county estimates for Mississippi. Surveillance, Epidemiology, and End Results (SEER) Program. https://statecancerprofiles.cancer.gov/incidencerates/index.php?stateFIPS=28&areatype=county&cancer=053&stage=211&race=00&sex=0&age=001&type=incd

# Search The Data & Methods


<!-- these are written in a combo of html and liquid --> 

<div class = "left">
{% include elements/button.html link="https://github.com/znquraishi/znquraishi.github.io/blob/main/_data/incd4.csv" text="The Data" %}
</div>

<div class="right">
{% include elements/button.html link="https://github.com/znquraishi/znquraishi.github.io/blob/main/python_notebooks/Final3.3_Workbook.ipynb" text="Analysis and Code for All Visualizations" %}
</div>

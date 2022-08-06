---
title: "Canada Gas"
date: 2020-06-08T08:06:25+06:00
description: Sample post with multiple images, embedded video ect.
menu:
  sidebar:
    name: Canada Gas
    identifier: PP-01
    parent: Pastime Projects
    weight: 301
hero: canada_gas.png
tags: ["Markdown","Content Organization","Multi-lingual"]
categories: ["Basic"]
---

<div align="left">
Lately drivers have been losing some sleep.<br>
The cost of gas has been quite steep.<p>

As rising prices are in our forecast.<br>
I wanted to see how they were in the past.<p>

I explore some data from the 90s to now.<br>
To try to gain some insights somehow.<p>

I go through some plots that I created,<br>
A few of them even animated.<p>

Interested in the plots displayed?<br>
Click here to see how they were made.<p>

You’ve read my intro. I’ve planted the seed.<br>
Now let’s get started. Enjoy the read!<p>

---


The main purpose of this article is to go through different methods of exploring time series data. The actual analysis will be very informal. All fuel prices were retrieved from [Statistics Canada](https://www150.statcan.gc.ca/t1/tbl1/en/tv.action?pid=1810000101). All monetary values are in Canadian dollars and have been adjusted to their present day (2022) dollar value.

Most plots were created using the [Plotly API](https://plotly.com/python-api-reference/) . Plotly allows users to create dynamic interactive plots and I especially like their animation feature when exploring time series data (I was not paid to write that and I have no affiliation with plotly at all). For the most ideal view of the plots please click on the bolded link at the bottom left corner of each display.


#### Line chart

The data used to create the line chart consists of monthly data from January 1990 to March 2022. There are 18 cities highlighted from 12 provinces and territories.

**Pros:** Line charts are usually useful for representing and gaining intuition on continuous data, especially as it changes over time. Estimates can be made as to the direction the data is heading and comparisons can be made between items to glean insights on relationships. A macro view of what is going on is probably the most prominent feature.

**Cons:** First looking at the plot, you can tell that quite a lot is going on. There are too many lines that have values that are too similar. This can make it challenging for an outside observer to make any significant comparisons.

**Tips to Interact:** Click and drag over any segment of the plot to get a zoomed in view of the line chart at any period in time. To zoom out, double click on the line chart. The buttons above give options to view the data at a specified window of time. Simply click on any of the buttons (1 month, 6 months…etc) and drag across the non-shaded portion of the slider at the bottom to pan through the line chart at the specified region of time. To hide a specific city, click on it in the legend to your right.
  
<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plotly.com/~jrkagumba/16.embed" height="570" width="100%"></iframe>

#### Choropleth Map

If you’re not Canadian, then there’s probably nothing odd about this choropleth map of Canada. However, the trained eye will notice that one of the territories is missing…Nunavut. Unfortunately there was no data available for Nunavut. Rather than just leaving it at zero and skewing the range of the colour bar, I decided to drop it altogether from the map…sorry Nunavut.

**Pros:** The general information about the data is visually effective. Someone who knows nothing about the data can see a large amount of information and discern some sort of general trend.

**Cons:** Since the choropleth map uses the mean price to represent defined provinces and territories, an observer cannot gain detailed information or perspective on any of the area’s internal status. Also, the gradient colours may not be distinct enough to be able to adequately distinguish differences in magnitude.

**Tips to Interact:** Click on the play and stop buttons at the bottom left to play through the animation. To manually explore a specific year, simply drag through the slider across to the desired year.
  
<iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plotly.com/~jrkagumba/2.embed" height="920" width="100%"></iframe>

#### Scatterplot

The data for the following scatter plot has been split by the yearly mean fuel price for each city. Yearly population data for each city was also added from [Statistics Canada](https://www.statcan.gc.ca/en/subjects-start/population_and_demography). From the population data, I also created the ‘Estimated Vehicles’ data point. It is simply the population size divided by 2… (I know that there is a more sophisticated way to calculate this, but for the purposes of this plot, that was adequate).

**Pros:** The scatter plot displays large quantities of data. It is easy to see what correlations exist between variables and the relevant clustering effects. Also, it’s quite simple to distinguish differences between maximum and minimum values within the data set.

**Cons:** It can be confusing to track all the variables being displayed and it’s easy to get lost in what is going on with each marker. This dataset specifically has quite a large discrepancy between population magnitudes and so a log axis had to be used.

**Tips to Interact:** Click and drag over any segment of the plot to get a zoomed-in view of the scatterplot. To zoom out, double click on the plot. To hide a specific city, click on it in the legend to your right. To manually explore a specific year, simply drag through the slider across to the desired year.
  
 <iframe id="igraph" scrolling="no" style="border:none;" seamless="seamless" src="https://plotly.com/~jrkagumba/14.embed" height="1140" width="100%"></iframe>

#### Racing Bar Chart

This is probably one of the most interesting and unique ways to display time series data. Racing bar charts have gained quite a bit of popularity over the last few years and have garnered quite a bit of attention in certain [YouTube](https://www.youtube.com/channel/UCkWbqlDAyJh2n8DN5X6NZyg) and [Reddit](https://www.reddit.com/r/dataisbeautiful/) communities. This particular bar chart was made with [Flourish](https://flourish.studio/examples/), and no code necessary.

**Pros:** This is obviously most effective when the data is continuous and there is a well defined maximum. Watching as items rise and fall in their value through time can be quite pleasing. There is an interesting visual narrative being portrayed in the data with a racing bar chart.

**Cons:** The bar charts are most concerned with rankings over time rather than actual item value. Tracking durational value trends of each item can be very difficult especially if the item goes out of view. This type of visualization is not ideal for showing the overall picture.

**Tips to Interact:** Click the pause and play button at the bottom left to pause or play. Click on any segment of the time line to visualize the data at that particular portion in time.

<div class="flourish-embed flourish-bar-chart-race" data-src="visualisation/8939322"><script src="https://public.flourish.studio/resources/embed.js"></script></div>

Each of these plots could be significantly expanded upon to provide further reasoning and clarity. If there’s any you’d like to discuss, hear more about, or disagree with let me know in the comments. The transformed data used to create these plots is available here.

#### References
[1] Statistics Canada - Monthly Prices for Gasoline by Geography<br>
[2] Statistics Canada - Population and Demography Statistics<br>
[3] Plotly API - Python API reference for Plotly<br>
[4] Flourish - Flourish Studio
---
title: "Sentiment Analysis from Twitter Data"
date: 2019-04-13
published: true
tags: [dataviz, altair, hvplot, holoviews]
excerpt: "Understanding trends in the sentiments around electric vehicles between 2015 and 2019"
altair-loader:
  altair-chart-1: "charts/measlesAltair.json"
hv-loader:
  hv-chart-1: ["charts/measlesHvplot.html", "500"] # second argument is the height
toc: false
toc_sticky: false
---


## Top 10 most common words gathered from tweets related to electric vehicles

![Fig1]({{ site.url }}{{ site.baseurl }}/assets/images/Fig1.png)

This was produced using Altair and embedded in this static web page. Note that you can also display Python code on this page:

```python
import altair as alt
alt.renderers.enable('notebook')
```

## HvPlot Example

Lastly, the measles incidence produced using the HvPlot package:

<div id="hv-chart-1"></div>

## Notes


---
layout: page
title: Datasets
permalink: /datasets/
description:
nav: true
nav_order: 3
display_categories: [work, fun]
horizontal: false
---


<style>
  .ucla-heading { color: #2774AE; }
</style>


<h3 class="ucla-heading">Indian Communal Violence Archive (ICVA)</h3>

<p>

The Indian Communal Violence Archive (ICVA) is a new event dataset covering
Hindu–Muslim communal violence across India from 2017 to 2024.
To build it, I collected and processed more than one million articles from the
<i>Times of India</i>, India's newspaper of record. I first used a BERT model as a high-recall filter to identify potentially relevant
articles before using generative large language models to classify reports of communal violence,
including incidents described through ambiguous language, euphemisms, or incomplete
reporting. I then extracted structured information about each incident, developed a
triangulation strategy to geolocate events from multiple partially overlapping reports,
and combined deterministic rules with LLM-assisted adjudication to merge duplicate
accounts of the same event. Finally, I linked every incident to India's administrative
and electoral geography. 
</p>

<h3 class="ucla-heading">Interactive Map</h3>

<p>
The map below links every recorded incident to India's Assembly Constituencies (ACs).
You can zoom and pan across the country, explore patterns of communal violence, and
click on individual constituencies to view recorded episodes. Each episodes includes
a short machine-assisted summary together with a direct link to the original
<i>Times of India</i> article, making it easy to quickly inspect and verify the
underlying source material.
</p>


<iframe
  src="{{ '/assets/html/leaflet_github_20260816.html' | relative_url }}"
  width="100%"
  height="850"
  style="border: none; border-radius: 8px;">
</iframe>

<br>

<h3 class="ucla-heading">Data Release</h3>

<p>
This archive is a work in progress. A companion paper describing its construction and validation is currently in preparation. The archive has not yet
been peer reviewed. Please do not use, redistribute, or cite the data without first contacting the author.
</p>

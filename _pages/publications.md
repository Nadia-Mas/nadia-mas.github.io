---
layout: page
permalink: /publications/
title: Publications
# description: publications by categories in reversed chronological order. generated by jekyll-scholar.
description: <h6>For the complete list, please see my <b><a href='https://scholar.google.com/citations?user=2uS4LM0AAAAJ&hl=en'>Google Scholar Profile</a></b>.</h6>
  # * indicates equal contribution
years: [2023, 2022, Thesis]
nav: true
nav_order: 1
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %}

</div>
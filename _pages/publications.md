---
layout: page
permalink: /publications/
title: Publications
description: Check the full publications <a href="https://scholar.google.com.hk/citations?user=HN6Y7z0AAAAJ&hl=en" target="_blank"><b>here</b></a>.
years: [2022, 2021, 2020, 2019, 2018]
nav: true
---

<div class="publications">

{% for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

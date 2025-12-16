---
layout: page
permalink: /publications/
title: publications
description: Selected publications. You can find a full list of publications in my Google Scholar.
years: [2025, 2024, 2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016]
nav: true
---

<!-- _pages/publications.md -->

<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers_sam -q @*[year={{y}}]* %}
{% endfor %}

</div>
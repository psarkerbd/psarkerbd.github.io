---
layout: page
permalink: /publications/
title: All Publications
description: This page lists my research publications in data compression, Huffman coding, adjacent distance array, and related computing areas. Each publication includes bibliographic details, indexing information, DOI/publisher link, abstract, and PDF where available.
years: [2024, 2022, 2021, 2020]
nav: false
nav_order: 
---
<!-- _pages/publications.md -->
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}
</div>

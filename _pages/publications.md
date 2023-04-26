---
layout: page
permalink: /publications/
title: Publications
description: The page provides information about the published content of the research. It includes a list of all published content in several journals or conferences, organized by date or category. Each entry in the list contains the title of the article or post, the name of the author, and the publication date. In addition, the page may retain a summary of each article or position and links to the full text.
years: [2022, 2021, 2020]
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

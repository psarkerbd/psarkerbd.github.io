---
layout: page
permalink: /publications/
title: Publications
description: The page provides information about the published content of the research. It includes a list of all accepted or published articles in several journals or conferences organized by date or category. In addition, the page may retain a summary of each article or position and associations to the full text.
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
<h6>Note:</h6>
<ol>
    <li id="footnote-1"> <b>*</b>  indicates the paper is accepted and entered into the publication schedule.</li>
</ol>
</div>

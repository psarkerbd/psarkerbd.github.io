---
layout: page
permalink: /publications/
title: Publications
description: The page provides information about the published content of the research. It includes a list of all published articles in several journals or conferences organized by date or category. Each entry in the list contains the title of the article or post, the name of the author, and the publication date. In addition, the page may retain a summary of each article or position and associations to the full text. Please note that I have another article, <a href='https://www.inderscience.com/info/ingeneral/forthcoming.php?jcode=ijict#111512' style="text-color:blue">A Huffman Based Short Message Service (SMS) Compression Technique Using Adjacent Distance Array</a>, that has been accepted and is yet to be published in <a href='https://www.inderscience.com/jhome.php?jcode=ijict'>International Journal of Information and Communication Technology</a>, a Scopus-indexed journal of <a href='https://www.inderscience.com/index.php'>Inderscience</a>.
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

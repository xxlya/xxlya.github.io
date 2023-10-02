---
layout: page
permalink: /publications/
title: publications
# description: Please check my full publication at <a href="https://scholar.google.com/citations?view_op=list_works&hl=en&hl=en&user=sdENOQ4AAAAJ&sortby=pubdate"> Google Scholar</a>
years: [2023, 2022, 2021]
nav: true
nav_order: 2
---
<div class="publications">

{%- for y in page.years %}
  <h2 class="year">{{y}}</h2>
  {% bibliography -f papers -q @*[year={{y}}]* %}
{% endfor %}

</div>

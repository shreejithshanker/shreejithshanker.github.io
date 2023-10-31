---
layout: page
permalink: /publications/
title: Publications
description: Below you will find a list of my publications and links to download them. Note that they are provided here to ensure timely dissemination of scholarly and technical work. Copyright and all rights therein are retained by authors or by other copyright holders.
years: [2023, 2022, 2021, 2020, 2019, 2018, 2017, 2016, 2015, 2014, 2013]
nav: true
nav_order: 1
---
You can also view my [Google Scholar](https://scholar.google.com/citations?hl=en&user=TySIJ-QAAAAJ),  and [ORCID](https://orcid.org/0000-0002-9717-1804) Profiles
<!-- _pages/publications.md -->
<div class="publications">

 {%- for y in page.years %}
  <h3 class="year">{{y}}</h3>
   {% bibliography -f {{ site.scholar.bibliography }} -q @*[year={{y}}]* %}
{% endfor %} 



</div>

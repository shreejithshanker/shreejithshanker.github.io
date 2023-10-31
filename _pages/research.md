---
layout: page
title: Research
permalink: /research/
description: 
nav: true
nav_order: 2
display_categories: [Research Team, Projects]
horizontal: false
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/wordcloud.png" title="Research" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    Research Tags
</div>

My research area focuses on building computer architectures that enable unique ways for improving compute efficiency, network performance and provide reactive capabilities to adapt to changing environments, through seamless interaction of software and hardware. 
I have applied this approach to tailor compute/network architectures in different domains such as automotive embedded systems, cognitive radio systems and internet of things. 
A key enabler for his research is fully programmable platforms (or reconfigurable hardware), which enables both the software and the underlying hardware to be adapted to the compute requirements and specifications, either statically (i.e., at design time) or dynamically (i.e., at run-time). 

Our current research focus is on enabling sustainable, adaptable and energy-efficient accelerators/digital designs for a range of data-driven tasks such as (light-weight) deep learning, media/video processing, communication networks and high-performance computing, among others. We investigate novel integration approaches, algorithmic and compiler optimisations and design space exploration schemes for co-designing and co-optimising applications with their accelerators. 

<!-- pages/projects.md -->
<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  {% if page.horizontal -%}
  <div class="container">
    <div class="row row-cols-2">
    {%- for project in sorted_projects -%}
      {% include projects_horizontal.html %}
    {%- endfor %}
    </div>
  </div>
  {%- else -%}
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {%- endif -%}
{%- endif -%}
</div>

## Current Masters Research Students ##
 * Oscar Toomey, Integrated Masters (MAI)
 * Peter O'Flynn, Integrated Masters (MAI)
 * Aparna Ramdoss, MSc Electronic Information Engineering
 * Changhong Li, MSc Electronic Information Engineering

## Former Students ##
 * Emmet Murphy, Integrated Masters, currently pursuing PhD at ETH, Zurich. 
 * Cornell Castelino, Integrated Masters, currently at [Analog Devices](https://analog.com), Ireland. 
 * Abhishek Dutta Gupta, MSc Electronic Information Engineering, starting PhD at Universidad Carlos III de Madrid (UC3M), Spain. 
 * Atul Redekar, MSc Electronic Information Engineering.
 * Daniel Flood, Integrated Masters, currently with [Geneva Trading](httpw://genevatrading.com), Dublin, Ireland. 
 * Jason Boyle, Integrated Masters, currently at [Microchip](https://microchip.com), Dublin, Ireland.
 * Nasir Said, Integrated Masters, currently at [Virtu Financial](https://virtu.com), Ireland. 
 * Aravind Raj, MSc Electronic Information Engineering, currently at [Synopsys](https://synopsys.com), Dublin.
 * Donal Lyons, Integrated Masters, currently at [SIG](https://sig.com), Dublin, Ireland 
 * Conor McNally Integrated Masters, currently at [AMD](https://amd.com), Dublin, Ireland. 
 * Eashan Wadhwa, Integrated Masters, currently at [Intel](https://intel.com), Ireland. 
 * Cian Wallnutt, Integrated Masters, currently at Coca-Cola, Ireland. 
 * Anushree Sawant, MSc Electronic Information Engineering, currently at [Intel](https://intel.com), Ireland. 
 * Siddhi Gaikwad, MSc Electronic Information Engineering, currently at [Intel](https://intel.com), Ireland. 
---
layout: page
title: research
permalink: /projects/
description: Trying to summarise the work I do!
nav: true
nav_order: 1
display_categories: [projects]
horizontal: false
---

<b>What are compact stars?</b>

Stars have a life cycle, living and dying based on how long they can push back against gravity. Gravity always acts inwards - wanting to collapse the star. This inward force of gravity has to be balanced by some sort of outward push. This is hydrostatic equilibrium.

"Main sequence" stars like the Sun achieve this through nuclear fusion. But fusion can only get us so far. Beyond iron, fusion is endothermic and the star can no longer stabilise itself against gravity. 

What happens next to the star is determined by its mass. A massive enough star is collapsed completely by gravity - this is when we get a <i>black hole</i>. Less massive stars can still achieve hydrostatic equilibrium - these end up as <i>white dwarfs</i> and <i>neutron stars</i>. 

These are the compact stars - the end-stages of a star's life. My research is focussed on this class of objects - and this page collects (semi-regularly) updated summaries of said work.

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

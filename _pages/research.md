---
layout: page
title: research
permalink: /research/
description: 
nav: true
nav_order: 3
display_categories: [Optimal Control, Intelligent Control, Others]
horizontal: false
---
## research vision

My research is positioned at the intersection of modern control theory, dynamic optimization, and robotics. My work spans two complementary directions: **optimal control**, including Model Predictive Control (MPC), reinforcement learning (RL), and deep reinforcement learning (DRL), and **intelligent control**, including direct adaptive fuzzy control (DAFC) and deep neural-network-based control — applied to control algorithms for robotic systems, including UAVs and other robot platforms, under nonlinear dynamics and disturbance.

A central objective of my work is to bridge control theory and practical implementation: deriving nonlinear plant models, designing controllers around them, and rigorously validating performance through MATLAB/Simulink simulation before any hardware deployment. Going forward, I'm looking to extend my optimal control work further into RL and DRL, and deepen my intelligent control work with deep neural network approaches, building controllers that can handle model uncertainty and generalize across robotic platforms and operating conditions, while keeping an eye on real-time computational feasibility.

My research activities are organized around the following themes.
# projects

<!-- This is additional, not the original version -->
<style>
.projects h2.category {
  text-align: left;
  color: var(--global-theme-color);
}
</style>

<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  <!-- change all project keyword to research, except projects_horizontal.liquid and projects.liquid -->
  {% for category in page.display_categories %}
  <a id="{{ category }}" href=".#{{ category }}">
    <h2 class="category">{{ category }}</h2>
  </a>
  {% assign categorized_research = site.research | where: "category", category %}
  {% assign sorted_research = categorized_research | sort: "importance" %}
  <!-- Generate cards for each project -->
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_research %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_research %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}

<!-- Display projects without categories -->
{% assign sorted_research = site.research | sort: "importance" %}
  <!-- Generate cards for each project -->
{% if page.horizontal %}

  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_research %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_research %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>

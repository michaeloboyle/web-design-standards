---
permalink: /
layout: styleguide
title: Government-wide Pattern Library
---

# About this Guide

This style guide is meant for as reference for designers, developers, as well as anyone else interested in the design and frontend concepts that make up the building blocks of federal government websites.

# Component name

<div class="preview">
<!-- Add HTML markup for example here -->
</div>

<div class="grid-box">
  <div class="grid-item width-one-half annotation">
    <h3>Use</h3>
    <p>This is where you'll find basic guidelines about the usage of a component. For example, a minimal palette, clear hierarchy, good information design, and ample whitespace will ensure a voice of authority and expertise in communication.</p>
  </div>
  <div class="grid-item width-one-half annotation">
    <h3>Accessibility</h3>
    <p>Accessibility is one of the most important aspects of modern web development. Accessibility means the greatest number of users can view your content.</p>
  </div>  
</div> 

# Visual Style

{% for visual in site.visual %}
## {{ visual.title }}
{{ visual.content }}
{% endfor %}

# Layout System

{% for layout in site.layout-system %}
## {{ layout.title }}

{{ layout.content }}
{% endfor %}

{% assign components = site.patterns | where:"type","component" %}
{% assign elements = site.patterns | where:"type","element" %}

# Elements

{% for element in elements %}
## {{ element.title }}
{{ element.content }}
{% endfor %}

# Components

{% for component in components %}
## {{ component.title }}
{{ component.content }}
{% endfor %}

<a href="#">Text link</a>

<button type="button">Button link</button>
---
layout: default
title: "Research"
permalink: /research/
---

# Research

I develop ultra-low-noise silicon detectors for astrophysics, enabling low-threshold dark matter searches and photon-counting observations in ground-based instruments and future space missions.

<nav class="research-toc">
  <strong>Jump to a topic</strong>
  {% assign items = site.research | sort: "date" | reverse %}
  {% for item in items %}
    <a href="#{{ item.title | slugify }}">{{ item.title }}</a>{% unless forloop.last %}&ensp;&middot;&ensp;{% endunless %}
  {% endfor %}
</nav>

---
{% assign items = site.research | sort: "date" | reverse %}
{% for item in items %}
<a id="{{ item.title | slugify }}" class="research-anchor"></a>


## {{ item.title }}

{{ item.content }}
{% endfor %}

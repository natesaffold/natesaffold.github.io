---
layout: default
title: "Teaching"
permalink: /teaching/
---

# Teaching and Outreach

I am committed to science education and public engagement through outreach programs for high school students and the broader public.

<nav class="research-toc">
  <strong>Jump to a topic</strong>
  {% assign items = site.teaching | sort: "date" | reverse %}
  {% for item in items %}
    <a href="#{{ item.title | slugify }}">{{ item.title }}</a>{% unless forloop.last %}&ensp;&middot;&ensp;{% endunless %}
  {% endfor %}
</nav>

---

{% assign items = site.teaching | sort: "date" | reverse %}
{% for item in items %}
<a id="{{ item.title | slugify }}" class="research-anchor"></a>

## {{ item.title }}

{% if item.venue or item.location %}
<p class="teaching-meta">
  {% if item.venue %}<strong>{{ item.venue }}</strong>{% endif %}
  {% if item.venue and item.location %} &mdash; {% endif %}
  {% if item.location %}{{ item.location }}{% endif %}
</p>
{% endif %}

{% if item.summary %}
<p class="research-summary">{{ item.summary }}</p>
{% endif %}

{{ item.content }}

<hr class="section-rule">
{% endfor %}

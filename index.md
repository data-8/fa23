---
layout: home
title: Home
nav_order: 1
nav_exclude: false
permalink: index.html
seo:
  type: Course
  name: Data 8 Fall 2023
---

# Data 8: Foundations of Data Science

{: .mb-2 }
UC Berkeley, Fall 2023
{: .mb-2 .fs-6 .text-grey-dk-000 }

## Announcements


{% assign announcements = site.announcements | reverse %}
{% for announcement in announcements %}
{{ announcement }}
{% endfor %}


{% assign mods = site.modules | where: 'class', 'Berkeley' %}
{% assign week1mods = '' | split: '' %}

{% for mod in mods %}
  {% if mod.title == 'Week 1' %}
    {% assign week1mods = week1mods | push: mod %}
  {% endif %}
{% endfor %}

{% for module in week1mods %}
  {{ module }}
{% endfor %}


<!--DARKMODE UNDER CONSTRUCTION-->
<br />



<p class="dm-text">The Data 8 Website Dark Mode&trade; is in beta. You can provide feedback about the website <a href="https://forms.gle/64xx2B1Y7K32bNhR9" class="yellow-link">here</a></p>



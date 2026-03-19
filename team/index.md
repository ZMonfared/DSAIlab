---
title: Team
nav:
  order: 1
  tooltip: About our team
---

<h1 style="font-weight: 800; font-size: 3em; text-align: center;">
  {% include icon.html icon="fa-solid fa-users" %} Team
</h1>

<div style="text-align: center;">
  In our lab, we value collaboration, equality, diversity and inclusion. We also respect our differences, and try to get the best out of it.
</div>

{% include section.html %}

<div style="text-align: center;">
  <img src="../images/our-team-image.jpg" alt="team photo" style="width: 85%; height: auto;"/>
</div>

{% include section.html %}

## Current Members

<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;">
  {% assign members = site.members | sort: "path" %}
  {% assign current = members | where_exp: "item", "item.group != 'alum'" %}
  {% for member in current %}
    {% include portrait.html data=member %}
  {% endfor %}
</div>

{% include section.html %}

## Former Members

<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;">
  {% assign alumni = site.members | where: "group", "alum" | sort: "path" %}
  {% for member in alumni %}
    {% include portrait.html data=member %}
  {% endfor %}
</div>

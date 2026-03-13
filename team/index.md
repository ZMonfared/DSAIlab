---
title: Team
nav:
  order: 1
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

<div style="text-align: center;">
  In our lab, we value collaboration, equality, diversity and inclusion. We also respect our differences, and try to get the best out of it.
</div>

{% include section.html %}

<div style="text-align: center;">
  <img src="../images/new_visitor_image.jpg" alt="team photo" style="width: 85%; height: auto;"/>
</div>

{% include section.html %}

## Current Members

<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;">
  {% assign current = site.members | rejectattr: "group", "equalto", "alum" %}
  {% for member in current %}
    {% include portrait.html data=member %}
  {% endfor %}
</div>

{% include section.html %}

## Former Members

<div style="display: flex; flex-wrap: wrap; gap: 20px; justify-content: center;">
  {% assign alumni = site.members | where: "group", "alum" %}
  {% for member in alumni %}
    {% include portrait.html data=member %}
  {% endfor %}
</div>

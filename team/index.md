---
title: Team
nav:
  order: 1
  tooltip: About our team
---

<style>
  /* Fix 1: Make the main heading bolder and larger */
  .big-heading {
    font-size: 3.5rem;
    font-weight: 900;
    margin-bottom: 20px;
    display: block;
  }

  /* Fix 2: Make the intro text larger */
  .intro-text {
    font-size: 1.4rem;
    font-weight: 400;
    line-height: 1.6;
    color: #333;
  }

  /* Fix 3: Change member icons from circle to square/rectangle */
  .portrait-image {
    border-radius: 4px !important; /* Change to 0px for sharp corners, or 4-8px for slightly rounded */
    aspect-ratio: 1 / 1; /* Ensures they stay square */
    object-fit: cover;
  }
</style>

<div style="text-align: center;">
  <h1 class="big-heading">
    {% include icon.html icon="fa-solid fa-users" %} Team
  </h1>
  
  <p class="intro-text">
    In our lab, we value collaboration, equality, diversity and inclusion. 
    We also respect our differences, and try to get the best out of it.
  </p>
</div>

{% include section.html %}

<div style="text-align: center;">
  <img src="../images/our-team-picture.jpeg" alt="team photo" style="width: 85%; height: auto;"/>
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

---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team
<div style="text-align: center;">
  In our lab, we value collaboration, equality, diversity, inclusion. We also respect our differences, and try to get best out of it
</div>
{% include section.html %}
<div style="text-align: center;">
  <img src="../images/5820970323481314659.jpg" alt="team photo" style="width: 50%; height: auto;"/>
</div>

{% include section.html %}

<div style="display: flex; overflow-x: auto; white-space: nowrap;">
  {% include list.html data="members" component="portrait" filter="role == 'pi'" %}
  {% include list.html data="members" component="portrait" filter="role != 'pi'" %}
</div>






---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
---

# {% include icon.html icon="fa-regular fa-envelope" %} Contact

Welcome! If you would like to reach out, please use the contact information below.

{%
  include button.html
  type="email"
  text="zahra.monfared@iwr.uni-heidelberg.de"
  link="mailto:zahra.monfared@iwr.uni-heidelberg.de"
%}
{%
  include button.html
  type="email"
  text="zahra.monfared@tum.de"
  link="mailto:zahra.monfared@tum.de"
%}
{%
  include button.html
  type="phone"
  text="+49 163 9176271"
  link="tel:+491639176271"
%}
{%
  include button.html
  type="address"
  tooltip="Our location on Google Maps for easy navigation"
  text="Dept. of Mathematics and Computer Science, IWR, Heidelberg University, Heidelberg, Germany"
  link="https://goo.gl/maps/HeidelbergUniversity"
%}
{%
  include button.html
  type="google-scholar"
  text="Google Scholar"
  link="https://scholar.google.pl/citations?user=OPUIwIoAAAAJ&hl=en"
%}

{% include section.html %}

{% capture col1 %}
**Contact Information**  
- **Email**: [zahra.monfared@iwr.uni-heidelberg.de](mailto:zahra.monfared@iwr.uni-heidelberg.de)  
- **Alternate Email**: [zahra.monfared@tum.de](mailto:zahra.monfared@tum.de)  
- **Phone**: [+49 163 9176271](tel:+491639176271)  
- **Location**: Dept. of Mathematics and Computer Science, IWR, Heidelberg University, Heidelberg, Germany  
- **Google Scholar**: [Link to Profile](https://scholar.google.pl/citations?user=OPUIwIoAAAAJ&hl=en)
{% endcapture %}

{% capture col2 %}
{%
  include figure.html
  image="images/group-image-corner.jpg"
  caption="Zahra Monfared, BMBF Research Group Leader"
  style="height: 100px;"
%}
{% endcapture %}

{% include cols.html col1=col1 col2=col2 %}

{% include section.html dark=true %}

{% capture col1 %}
Stay connected for more research updates and collaborations.
{% endcapture %}

{% capture col2 %}
Looking forward to engaging with the research community.
{% endcapture %}

{% capture col3 %}
Thank you for visiting my contact page!
{% endcapture %}

{% include cols.html col1=col1 col2=col2 col3=col3 %}

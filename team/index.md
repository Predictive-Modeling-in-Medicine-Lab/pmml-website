---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %}Team

Our lab is highly interdisciplinary and collaborative. We bring together expertise from a range of different areas, including computational science and engineering, biomedical engineering, physiology, medicine, and scientific software development.

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'principal-investigator'" %}
{% include list.html data="members" component="portrait" filter="role == 'research-associate'" %}
{% include list.html data="members" component="portrait" filter="role == 'postdoc'" %}
{% include list.html data="members" component="portrait" filter="role == 'phd'" %}



{% include section.html %}
# {% include icon.html icon="fa-solid fa-handshake" %} Supporters
Our work would not be possible without the support of the following organizations.
{% include section.html %}
{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}

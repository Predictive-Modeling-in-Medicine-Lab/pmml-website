---
title: Contact
nav:
  order: 5
  tooltip: Email, address, and location
background: images/backgrounds/anschutz.jpg
---

# {% include icon.html icon="fa-regular fa-envelope" %}Contact

Our lab is part of the [University of Texas at Austin](https://www.utexas.edu/)'s [Center for Computational Medicine](https://oden.utexas.edu/research/centers-and-groups/center-for-computational-medicine/). We are based jointly within the [Oden Institute for Computational Engineering and Sciences](https://oden.utexas.edu/) and the [Dell Medical School](https://dellmed.utexas.edu/).
{% capture content %}
{%
  include figure.html
  image="images/ut.png"
  link="https://utexas.edu/"
  width="400px"
%}
{%
  include figure.html
  image="images/oden.png"
  link="https://oden.utexas.edu/"
  width="400px"
%}
{%
  include figure.html
  image="images/DellMed.png"
  link="https://dellmed.utexas.edu/"
  width="400px"
%}

{% endcapture %}

{% include grid.html style="row" content=content %}


{%
  include button.html
  type="email"
  text=site.links.email
  link=site.links.email
%}
{%
  include button.html
  type="address"
  text= "Address: 4th Floor, Peter O'Donnell, Jr. Building, UT Austin"
  tooltip="Our location on Google Maps for easy navigation"
  link="https://maps.app.goo.gl/2pBTEZnsrsy6dGGV9"
%}

{% capture content %}
{% include figure.html image="images/contact/ut.jpg" %}
{% include figure.html image="images/contact/pob.jpg" %}
{% include figure.html image="images/contact/posters.jpg" %}
{% endcapture %}

{%
  include grid.html
  content=content
  style="square"
%}
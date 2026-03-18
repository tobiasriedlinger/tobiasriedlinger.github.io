---
layout: default
title: Publications
description: 
---

{% include nav.html %}

A full list can be found on my  
[Google Scholar](https://scholar.google.de/citations?user=XggH5bwAAAAJ).

{% assign pubs = site.data.publications | sort: "year" | reverse %}

## Selected
<!-- > **Towards Reliable Detection of Empty Space: Conditional Marked Point Processes for Object Detection**
> Tobias Riedlinger, Kira Maag and Hanno Gottschalk

> **Lmd: Light-weight prediction quality estimation for object detection in lidar point clouds**
> Tobias Riedlinger, Marius Schubert, Sarina Penquitt, Jan-Marcel Kezmann, Pascal Colling, Karsten Kahl, Lutz Roese-Koerner, Michael Arnold, Urs Zimmermann, and Matthias Rottmann

> **Gradient-Based Quantification of Epistemic Uncertainty for Deep Object Detectors**
> Tobias Riedlinger, Matthias Rottmann, Marius Schubert, and Hanno Gottschalk -->

{% for pub in pubs %}
  {% if pub.selected %}
**{{ pub.title }}**  
{{ pub.authors }}  
*{{ pub.venue }}*, {{ pub.year }}  
{% if pub.url %}[Paper]({{ pub.url }}){% endif %}

  {% endif %}
{% endfor %}

## Full List

{% assign years = pubs | map: "year" | uniq %}

{% for y in years %}
## {{ y }}

  {% for pub in pubs %}
    {% if pub.year == y %}
**{{ pub.title }}**  
{{ pub.authors }}  
*{{ pub.venue }}*  
{% if pub.url %}[Paper]({{ pub.url }}){% endif %}

    {% endif %}
  {% endfor %}
{% endfor %}
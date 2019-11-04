---
layout: project
title: "Geocoding Early Novels"
authors: ['inachen', 'cassidyholahan', 'dorothypierrelouis']
tags: [projects]
img: geocoding_map.jpg
description:
display-order: 1
---



Geocoding Early Novels is a collaborative project completed in the summer of 2019 that maps specific locations mentioned in the title pages of novels from the long eighteenth century. We were able to map 943 locations from 2,002 catalogued novels. This project was conceived of and executed by the 2019 Summer END team: Ina Chen, Cassidy Holahan, and Dorothy Pierre-Louis.

The project can be found [here](https://cholahan.github.io/end19/).

{% for a in page.authors %}
{% assign author = site.data.authors[a] %}
{% include author.html author=author %}
{% endfor %}

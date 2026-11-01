---
layout: default
title: Faktenbilanz – Quellen
---

# Faktenbilanz – Quellen

Nachgerechnet. Belegt. Hier stehen die vollständigen Quellen zu jedem Video von [@faktenbilanz](https://www.youtube.com/@faktenbilanz).

{% assign seiten = site.pages | where: "quelle", true | sort: "title" %}
{% for p in seiten %}- [{{ p.title | remove: "Quellen: " }}]({{ p.url | relative_url }})
{% endfor %}

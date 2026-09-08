---
layout: academic
title: Sitemap
permalink: /sitemap/
---

- [Home]({{ '/' | relative_url }})
- [Publications]({{ '/publications/' | relative_url }})
- [Brief CV]({{ '/cv/' | relative_url }})

## Papers

{% for paper in site.publications reversed %}
- [{{ paper.title }}]({{ paper.url | relative_url }})
{% endfor %}

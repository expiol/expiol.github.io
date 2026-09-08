---
layout: academic
title: Brief CV
permalink: /cv/
redirect_from:
  - /resume
---

<p class="page-lead">Yang Hong · Building a startup · AI &amp; cybersecurity research</p>

<section class="home-section" aria-labelledby="cv-education"><h2 id="cv-education">Education</h2>
{% include academic/education.html %}
</section>

<section class="home-section" aria-labelledby="cv-research"><h2 id="cv-research">Research Experience</h2>
{% include academic/experience.html items=site.data.academic.research compact=true %}
</section>

<section class="home-section" aria-labelledby="cv-industry"><h2 id="cv-industry">Industry Experience</h2>
{% include academic/experience.html items=site.data.academic.internships compact=true %}
</section>

<section class="home-section" aria-labelledby="cv-publications"><h2 id="cv-publications">Publications</h2>
{% assign papers = site.publications | sort: 'date' | reverse %}
<ul class="cv-paper-list">
{% for paper in papers %}
  <li><a href="{{ paper.url | relative_url }}">{{ paper.title }}</a><span class="entry-meta">{{ paper.venue_short }} · {{ paper.date | date: '%Y' }}</span></li>
{% endfor %}
</ul>
<p><a href="{{ '/publications/' | relative_url }}">Full publication details →</a></p>
</section>

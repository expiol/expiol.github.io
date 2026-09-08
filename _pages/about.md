---
layout: academic
permalink: /
title: "Yang Hong | Entrepreneurship & AI Security"
home: true
description: "Yang Hong is building a startup, with a research background in AI and cybersecurity. Incoming M.S. student in Security Informatics at Johns Hopkins University."
redirect_from:
  - /about/
  - /about.html
---

<section class="intro" aria-labelledby="about-heading">
  <p class="eyebrow">ENTREPRENEURSHIP &amp; RESEARCH</p>
  <h1 id="about-heading">Hi, I'm Yang Hong.</h1>
  <p>I am currently <strong>building a startup</strong>, with a research background in <strong>AI and cybersecurity</strong>.</p>
  <p>My research focuses on language model safety and privacy, the security of multi-agent systems, and automated penetration testing. I am interested in both understanding the risks of AI systems and exploring their use in practical security workflows.</p>
  <p>I received my bachelor's degree in Information and Computing Science from <a href="https://www.xjtlu.edu.cn/en/">Xi'an Jiaotong-Liverpool University</a> in 2026. I am an incoming M.S. student in Security Informatics at <a href="https://www.jhu.edu/">Johns Hopkins University</a>.</p>
  <p>My research on LLM security includes work co-authored with <a href="https://www.cs.jhu.edu/faculty/yinzhi-cao/">Prof. Yinzhi Cao</a> and Ph.D. student Rui Yang at Johns Hopkins University. Previously, I worked with Prof. Wenjun Fan at XJTLU on LLM-assisted Capture-the-Flag solving.</p>
  <div class="research-interests" aria-label="Research interests"><span>LLM safety &amp; privacy</span><span>Multi-agent security</span><span>Automated pentesting</span></div>
</section>

<section class="home-section news-section" aria-labelledby="news-heading">
  <h2 id="news-heading">News</h2>
  <ul class="news-list">
    <li><time datetime="2026-09">Sep 2026</time><span>Two new preprints: <a href="https://arxiv.org/abs/2609.00578">cybersecurity assistance across conversational contexts</a> and <a href="https://arxiv.org/abs/2609.00595">the security of multi-agent LLM systems</a>.</span></li>
  </ul>
</section>

<section id="publications" class="home-section" aria-labelledby="publications-heading">
  <div class="section-heading"><h2 id="publications-heading">Publications</h2><a class="section-link" href="{{ '/publications/' | relative_url }}">All papers <span aria-hidden="true">→</span></a></div>
  {% include academic/publications.html %}
</section>

<section id="experience" class="home-section" aria-labelledby="experience-heading">
  <h2 id="experience-heading">Research Experience</h2>
  {% include academic/experience.html items=site.data.academic.research %}
  <h3 class="subsection-heading">Industry Experience</h3>
  {% include academic/experience.html items=site.data.academic.internships %}
</section>

<section id="education" class="home-section" aria-labelledby="education-heading">
  <h2 id="education-heading">Education</h2>
  {% include academic/education.html %}
</section>

<section id="contact" class="home-section contact-section" aria-labelledby="contact-heading">
  <h2 id="contact-heading">Get in touch</h2>
  <p>For research discussions and collaboration, reach me at <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a>.</p>
</section>

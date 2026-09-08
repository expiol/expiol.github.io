---
layout: academic
permalink: /
title: "Yang Hong | Entrepreneurship & AI Security"
home: true
description: "Yang Hong is building a startup and researching AI security: language model safety, multi-agent systems, and automated penetration testing. Incoming M.S. student at Johns Hopkins University."
redirect_from:
  - /about/
  - /about.html
---

<section class="intro" aria-labelledby="about-heading">
  <p class="eyebrow">ENTREPRENEURSHIP &amp; RESEARCH</p>
  <h1 id="about-heading">Hi, I'm Yang Hong.</h1>
  <p>I am currently <strong>building a startup</strong>, with a research background in <strong>AI and cybersecurity</strong>.</p>
  <p>I work on language model safety and privacy, the security of multi-agent systems, and automated penetration testing &mdash; both understanding where AI systems fail and putting them to work in real security tasks.</p>
  <p>I received my bachelor's degree in Information and Computing Science from <a href="https://www.xjtlu.edu.cn/en/">Xi'an Jiaotong-Liverpool University</a> in 2026, and am an incoming M.S. student in Security Informatics at <a href="https://www.jhu.edu/">Johns Hopkins University</a>.</p>
  <p>My LLM security work is a collaboration with Ph.D. student Rui Yang at Johns Hopkins, co-authored with <a href="https://www.cs.jhu.edu/faculty/yinzhi-cao/">Prof. Yinzhi Cao</a>. Earlier, I worked with Prof. Wenjun Fan at XJTLU on LLM-assisted Capture-the-Flag solving.</p>
  <div class="research-interests" aria-label="Research interests">{% for interest in site.author.interests %}<span>{{ interest }}</span>{% endfor %}</div>
</section>

<section class="home-section news-section" aria-labelledby="news-heading">
  <h2 id="news-heading">News</h2>
  <ul class="news-list">
    <li><time datetime="2026-09">Sep 2026</time><span>Two new preprints: <a href="https://arxiv.org/abs/2609.00578">cybersecurity assistance across conversational contexts</a> and <a href="https://arxiv.org/abs/2609.00595">the security of multi-agent LLM systems</a>.</span></li>
    <li><time datetime="2026-07">Jul 2026</time><span><a href="{{ '/publication/2026-pentestllm/' | relative_url }}">PentestLLM</a>, a kill chain-driven multi-agent framework for automated penetration testing, published at COMPSAC 2026.</span></li>
    <li><time datetime="2024-12">Dec 2024</time><span>Our work on <a href="{{ '/publication/2024-trustcom-ctf-llm/' | relative_url }}">LLM agents for Capture-the-Flag challenge solving</a> published at TrustCom 2024.</span></li>
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
  <p>I am always glad to talk about AI security research and potential collaboration. The fastest way to reach me is email: <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a>.</p>
</section>

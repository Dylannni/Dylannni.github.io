---
permalink: /
title: null
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% include base_path %}

## Welcome!

I am **Zehao (Dylan) Lin**, a BSc Computer Science student at the University of Bristol.

- Backend Intern at Tencent (Summer 2025)
- Co-Founder and President at Bristol Formula Student AI
- Interested in multimodal machine learning and production backend systems

## Recent Work

- Built an ad delivery pipeline at Tencent handling **600K+ QPS**.
- Reduced deployment latency from **8 minutes to 2 minutes** on AWS EKS.
- Achieved **Top 10%** (2000+ teams) in Tencent Advertising Algorithms Competition.

## Featured Projects

{% assign featured_projects = site.portfolio | sort: "date" | reverse %}
{% if featured_projects.size > 0 %}
<ul>
{% for post in featured_projects limit: 3 %}
  <li>
    <a href="{{ base_path }}{{ post.url }}">{{ post.title }}</a>
    {% if post.excerpt %}
    - {{ post.excerpt | markdownify | strip_html | strip_newlines }}
    {% endif %}
  </li>
{% endfor %}
</ul>
{% else %}
No projects yet. Add items under the `_portfolio` folder.
{% endif %}

[View all projects]({{ base_path }}/projects/)

## Experience Snapshot

- Backend Intern at Tencent, where I helped build an ad delivery pipeline handling 600K+ QPS.
- Reduced deployment latency from 8 minutes to 2 minutes by improving containerized CI/CD on AWS EKS.
- Co-founded Bristol Formula Student AI and led a 50-member team building an autonomous driving system.

[See full experience]({{ base_path }}/experience/)

## Blogs

I use this section to write technical notes and project reflections.

[View all blogs]({{ base_path }}/blogs/)

## Visitor Map

<div style="margin-top: 0.5rem; text-align: center;">
  <script
    type="text/javascript"
    id="mapmyvisitors"
    src="https://mapmyvisitors.com/map.js?d=oc2H0Wc6hZN5ompE5XYLlgr_zhkGMaKqJlwayt7w690&cl=ffffff&w=a">
  </script>
  <noscript>
    <a href="https://mapmyvisitors.com/web/1c2y9" title="Visit tracker">
      <img src="https://mapmyvisitors.com/map.png?d=oc2H0Wc6hZN5ompE5XYLlgr_zhkGMaKqJlwayt7w690&cl=ffffff" alt="Visitor map" />
    </a>
  </noscript>
</div>

Open full stats on [MapMyVisitors](https://mapmyvisitors.com/web/1c2y9).

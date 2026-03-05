---
permalink: /
title: null
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% include base_path %}

## About Me

Hi, I'm **Zehao (Dylan) Lin**, a final-year Computer Science student at the University of Bristol. I interned at Tencent where I built ad-serving infrastructure handling 600K+ QPS, and co-founded Bristol Formula Student AI — leading a 50-member team building an autonomous driving system. I also won Apple's Swift Student Challenge as a Distinguished Winner (Top 50 Worldwide).

I'm interested in production backend systems and multimodal video understanding and egocentric vision.

## Featured Projects

{% assign featured_projects = site.portfolio | sort: "date" | reverse %}
{% if featured_projects.size > 0 %}
<ul>
{% for post in featured_projects limit: 2 %}
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

## Experience

[See full experience]({{ base_path }}/experience/)

## Visitor Map

<div style="margin-top: 0.5rem; text-align: center; max-width: 480px; border: 1px solid var(--global-border-color); border-radius: 10px; padding: 1rem;">
  <script
    type="text/javascript"
    id="mapmyvisitors"
    src="//mapmyvisitors.com/map.js?d=oc2HOWc6hZN5ompE5XYLlgr_zhkGMaKqJlWayt7w690&cl=ffffff&w=a">
  </script>
  <noscript>
    <a href="https://mapmyvisitors.com/web/1c2y9" title="Visit tracker">
      <img src="https://mapmyvisitors.com/map.png?d=oc2HOWc6hZN5ompE5XYLlgr_zhkGMaKqJlWayt7w690&cl=ffffff" alt="Visitor map" />
    </a>
  </noscript>
</div>

Open full stats on [MapMyVisitors](https://mapmyvisitors.com/web/1c2y9).

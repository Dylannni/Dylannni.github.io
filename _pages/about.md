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

Hi, I'm **Zehao (Dylan) Lin**, a Founding Member of Technical Staff at [Memories.ai](https://memories.ai), where I work on the Large Visual Memory Model (LVMM). My focus is egocentric video understanding and 3D human motion reconstruction, including 3D hand pose and 6DoF head pose estimation, taking research all the way to a production pipeline running on 1M+ hours of video. I'm also pursuing an MSE in Artificial Intelligence at the University of Pennsylvania.

I graduated from the University of Bristol with a First Class BSc in Computer Science. Before that, I interned at Tencent, building ad-serving infrastructure handling 600K+ QPS, and co-founded Bristol Formula Student AI, leading a 50-member team whose autonomous driving system completed three fully autonomous laps at Silverstone and earned the team's first-ever dynamic points. I was also a Distinguished Winner (Top 50 Worldwide) of Apple's Swift Student Challenge.

I'm interested in egocentric vision, 3D human motion reconstruction, and multimodal video understanding.

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

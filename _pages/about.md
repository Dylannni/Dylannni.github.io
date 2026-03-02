---
permalink: /
title: "Zehao (Dylan) Lin"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% include base_path %}

I am a BSc Computer Science student at the University of Bristol.

I build backend systems and AI-enabled products, with interests in multimodal machine learning and reliable production infrastructure.

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

## Recent Blogs

{% if site.posts.size > 0 %}
{% for post in site.posts limit: 3 %}
  {% include archive-single.html %}
{% endfor %}
{% else %}
No posts yet. This section is ready for your technical writeups.
{% endif %}

[View all blogs]({{ base_path }}/blogs/)

## Contact

- Phone: +44 7539 982259
- Email: [{{ site.author.email }}](mailto:{{ site.author.email }})
- GitHub: [{{ site.author.github }}](https://github.com/{{ site.author.github }})
- LinkedIn: [{{ site.author.linkedin }}](https://www.linkedin.com/in/{{ site.author.linkedin }})

## Visitor Map

<div style="margin-top: 0.5rem;">
  <iframe
    title="Visitor map"
    src="https://clustrmaps.com/site/1c12r"
    loading="lazy"
    style="width: 100%; max-width: 820px; height: 320px; border: 0;">
  </iframe>
</div>

If the embed does not load, open the full map on [ClustrMaps](https://clustrmaps.com/site/1c12r).

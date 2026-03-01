---
permalink: /
title: "Zehao (Dylan) Lin"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

{% include base_path %}

I build backend systems and AI-enabled products.

Currently focused on distributed services, practical ML integration, and shipping production-ready features.

## Featured Projects

<div class="grid__wrapper">
{% assign featured_projects = site.portfolio | sort: "date" | reverse %}
{% for post in featured_projects limit: 3 %}
  {% include archive-single.html type="grid" %}
{% endfor %}
</div>

[View all projects]({{ base_path }}/projects/)

## Experience Snapshot

- Backend and platform engineering experience across internship and academic projects.
- Focus on API design, data pipelines, and service reliability.
- Comfortable moving from prototype to production.

[See full experience]({{ base_path }}/experience/)

## Recent Writing

{% if site.posts.size > 0 %}
{% for post in site.posts limit: 3 %}
  {% include archive-single.html %}
{% endfor %}
{% else %}
No posts yet. This section is ready for your technical writeups.
{% endif %}

[View all writing]({{ base_path }}/writing/)

## Contact

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

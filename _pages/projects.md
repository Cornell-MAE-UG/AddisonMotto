---
layout: default
title: Projects
description: Selected mechanical engineering, research, and design projects by Addison Motto.
permalink: /projects/
---

<section class="page-intro site-shell">
  <p class="eyebrow">Project index</p>
  <h1>Design, analysis, and hardware brought into the real world.</h1>
  <p>Selected work across mechanical systems, aerodynamics, manufacturing, and robotics research.</p>
</section>

<section class="project-index site-shell">
  {% assign projects = site.projects | sort: "order" %}
  {% for project in projects %}
    <article class="index-row">
      <a class="index-image" href="{{ project.url | relative_url }}">
        <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" loading="lazy">
      </a>
      <p class="project-number">0{{ forloop.index }}</p>
      <div class="index-copy">
        <p class="project-kicker">{{ project.description }}</p>
        <h2><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h2>
        <p>{{ project.summary | default: project.excerpt | strip_html | truncatewords: 38 }}</p>
        <div class="tag-list">
          {% for technology in project.technologies %}<span>{{ technology }}</span>{% endfor %}
        </div>
      </div>
      <a class="round-link" href="{{ project.url | relative_url }}" aria-label="View {{ project.title }}">&#8599;</a>
    </article>
  {% endfor %}
</section>

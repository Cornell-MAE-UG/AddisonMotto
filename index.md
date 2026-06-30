---
layout: default
title: Addison Motto
description: Mechanical engineer focused on design, prototyping, testing, and multidisciplinary systems.
---

<section class="hero site-shell">
  <div class="hero-copy">
    <p class="eyebrow">Mechanical engineer &middot; Cornell University</p>
    <h1>About me</h1>
    <p class="hero-intro">My name is Addison Motto, and I recently graduated magna cum laude from Cornell University with a degree in Mechanical Engineering. I am currently pursuing a Master of Engineering in Systems Engineering, with interests in designing, analyzing, and building complex engineering systems from early concepts and CAD to prototyping, testing, and real-world implementation. My experience spans electric vehicles, aerospace and defense hardware, manufacturing, and product development, and I enjoy work that combines hands-on engineering, system-level thinking, and creative problem solving.</p>
    <div class="hero-actions">
      <a class="button button-primary" href="#featured-work">See featured work <span aria-hidden="true">&#8595;</span></a>
      <a class="text-link" href="{{ "/assets/Resume.pdf" | relative_url }}" target="_blank" rel="noopener">Open resume <span aria-hidden="true">&#8599;</span></a>
    </div>
  </div>
  <figure class="portrait-wrap">
    <img src="{{ "/assets/images/addison-wind-turbine.png" | relative_url }}" alt="Addison Motto standing beside the interactive wind turbine exhibit he helped engineer">
    <figcaption>Design &middot; Analysis &middot; Prototyping</figcaption>
  </figure>
</section>

<section class="signal-band">
  <div class="site-shell signal-grid">
    <p class="eyebrow">Core engineering focus</p>
    <div class="signal-list" aria-label="Core engineering skills">
      <span>Mechanical design</span>
      <span>CAD &amp; GD&amp;T</span>
      <span>Simulation &amp; modeling</span>
      <span>Prototyping</span>
      <span>Testing &amp; validation</span>
    </div>
  </div>
</section>

<section id="featured-work" class="section site-shell">
  <div class="section-heading">
    <div>
      <p class="eyebrow">01 &middot; Selected work</p>
      <h2>Selected engineering work.</h2>
    </div>
    <p>Projects spanning public-facing hardware, aerodynamic optimization, and insect-scale robotics.</p>
  </div>

  <div class="featured-projects">
    {% assign featured = site.projects | sort: "order" %}
    {% for project in featured %}
      <article class="featured-project">
        <a class="project-media" href="{{ project.url | relative_url }}">
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" loading="{% if forloop.first %}eager{% else %}lazy{% endif %}">
        </a>
        <div class="project-summary">
          <p class="project-number">0{{ forloop.index }}</p>
          <div>
            <p class="project-kicker">{{ project.description }}</p>
            <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
            <p>{{ project.summary | default: project.excerpt | strip_html | truncatewords: 31 }}</p>
            <div class="tag-list">
              {% for technology in project.technologies %}<span>{{ technology }}</span>{% endfor %}
            </div>
          </div>
          <a class="round-link" href="{{ project.url | relative_url }}" aria-label="View {{ project.title }}">&#8599;</a>
        </div>
      </article>
    {% endfor %}
  </div>

  <div class="section-action">
    <a class="button button-outline" href="{{ "/projects/" | relative_url }}">Browse all projects <span aria-hidden="true">&#8594;</span></a>
  </div>
</section>

<section class="personal-band">
  <div class="site-shell personal-grid">
    <div class="personal-copy">
      <p class="eyebrow">02 &middot; Personal interests</p>
      <h2>Always moving, learning, and finding the next place to explore.</h2>
      <p>Outside engineering, I spend a lot of time skiing, running, hiking, and traveling. I love trying new things, getting outside whenever I can, and bringing that same curiosity and energy into the way I approach projects.</p>
      <a class="text-link" href="{{ "/Resume/" | relative_url }}">Experience and education <span aria-hidden="true">&#8594;</span></a>
    </div>
    <div class="interest-gallery" aria-label="Personal interests">
      <figure class="interest-card interest-card-tall">
        <img src="{{ "/assets/images/addison-skiing.png" | relative_url }}" alt="Addison skiing through deep snow" loading="lazy">
      </figure>
      <figure class="interest-card">
        <img src="{{ "/assets/images/addison-running.png" | relative_url }}" alt="Addison after finishing a run" loading="lazy">
      </figure>
      <figure class="interest-card">
        <img src="{{ "/assets/images/addison-hiking.png" | relative_url }}" alt="Addison hiking in a snowy mountain landscape" loading="lazy">
      </figure>
    </div>
  </div>
</section>

---
title: Home
description: Power electronics research at Nantong University.
---

<div class="home-hero" style="--hero-image: url('{{ "images/background.jpg" | relative_url }}')">
  <div class="home-hero__content">
    <p class="eyebrow">Power Electronics Laboratory · Nantong University</p>
    <h1>Engineering the future of electrical energy.</h1>
    <p class="home-hero__lead">We investigate efficient power conversion, intelligent control, and enabling technologies for more sustainable energy systems.</p>
    <a class="home-hero__link" href="{{ "/research/" | relative_url }}">Explore our research <span aria-hidden="true">→</span></a>
  </div>
</div>

<div class="home-intro page-shell">
  <p class="section-label">About the laboratory</p>
  <div class="home-intro__grid">
    <h2>Power electronics for a more efficient and electrified world.</h2>
    <div>
      <p>The Power Electronics Laboratory at Nantong University brings together research in power conversion, control, and energy systems. Our work connects fundamental engineering questions with practical challenges in modern electrification.</p>
      <p>We pursue rigorous research, hands-on experimentation, and collaboration across disciplines.</p>
    </div>
  </div>
</div>

<div class="home-news page-shell">
  <div class="section-heading">
    <div>
      <p class="section-label">News &amp; events</p>
      <h2>Latest from the laboratory</h2>
    </div>
    <a href="{{ "/blog/" | relative_url }}">View all news <span aria-hidden="true">→</span></a>
  </div>

  <div class="news-grid">
    {% for post in site.posts limit: 3 %}
      <article class="news-card">
        <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%d %B %Y" }}</time>
        <h3><a href="{{ post.url | relative_url }}">{{ post.title }}</a></h3>
        <p>{{ post.content | strip_html | truncatewords: 24 }}</p>
        <a class="text-link" href="{{ post.url | relative_url }}" aria-label="Read {{ post.title }}">Read more <span aria-hidden="true">→</span></a>
      </article>
    {% endfor %}
  </div>
</div>

<div class="research-feature">
  <div class="research-feature__image" role="img" aria-label="Abstract visualization representing power electronics research" style="--feature-image: url('{{ "images/background.jpg" | relative_url }}')"></div>
  <div class="research-feature__content">
    <p class="section-label">Research</p>
    <h2>From devices and converters to complete energy systems.</h2>
    <p>Our research explores the technologies and system-level ideas needed to convert, control, and use electrical energy with greater performance and efficiency.</p>
    <a href="{{ "/research/" | relative_url }}">Discover our research <span aria-hidden="true">→</span></a>
  </div>
</div>

<div class="home-pathways page-shell">
  <p class="section-label">Explore the laboratory</p>
  <div class="pathway-grid">
    <a class="pathway" href="{{ "/research/" | relative_url }}">
      <span class="pathway__number">01</span>
      <h2>Research</h2>
      <p>Explore publications and the questions that guide our work.</p>
      <span class="pathway__arrow" aria-hidden="true">→</span>
    </a>
    <a class="pathway" href="{{ "/projects/" | relative_url }}">
      <span class="pathway__number">02</span>
      <h2>Projects</h2>
      <p>See our current platforms, prototypes, and collaborative efforts.</p>
      <span class="pathway__arrow" aria-hidden="true">→</span>
    </a>
    <a class="pathway" href="{{ "/team/" | relative_url }}">
      <span class="pathway__number">03</span>
      <h2>Team</h2>
      <p>Meet the researchers and students behind the laboratory.</p>
      <span class="pathway__arrow" aria-hidden="true">→</span>
    </a>
  </div>
</div>

<div class="home-contact page-shell">
  <p class="section-label">Connect</p>
  <h2>Interested in our work?</h2>
  <p>Learn more about the laboratory, our research, and opportunities to collaborate.</p>
  <a href="{{ "/contact/" | relative_url }}">Contact the laboratory <span aria-hidden="true">→</span></a>
</div>

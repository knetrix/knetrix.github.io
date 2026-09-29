---
layout: default
title: Docker
permalink: /tutorials/docker/
---
<section class="course-header">
  <h1>Docker</h1>
  <p>Containers, images, Compose, networking, and deployment basics.</p>
</section>
<section class="lesson-list" aria-label="Docker lessons">
{% assign lessons = site.tutorials | where: "course", "docker" | sort: "order" %}
{% for lesson in lessons %}
  <a class="lesson-card" href="{{ lesson.url | relative_url }}"><span class="lesson-order">{{ lesson.order | prepend: '0' | slice: -2, 2 }}</span><span><h2>{{ lesson.title }}</h2>{% if lesson.excerpt %}<p>{{ lesson.excerpt }}</p>{% endif %}</span></a>
{% else %}
  <p class="empty-state">Lessons for this course are coming soon.</p>
{% endfor %}
</section>

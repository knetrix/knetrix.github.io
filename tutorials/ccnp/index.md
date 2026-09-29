---
layout: default
title: CCNP
permalink: /tutorials/ccnp/
---
<section class="course-header">
  <h1>CCNP</h1>
  <p>Enterprise networking concepts and advanced routing and switching.</p>
</section>
<section class="lesson-list" aria-label="CCNP lessons">
{% assign lessons = site.tutorials | where: "course", "ccnp" | sort: "order" %}
{% for lesson in lessons %}
  <a class="lesson-card" href="{{ lesson.url | relative_url }}"><span class="lesson-order">{{ lesson.order | prepend: '0' | slice: -2, 2 }}</span><span><h2>{{ lesson.title }}</h2>{% if lesson.excerpt %}<p>{{ lesson.excerpt }}</p>{% endif %}</span></a>
{% else %}
  <p class="empty-state">Lessons for this course are coming soon.</p>
{% endfor %}
</section>

---
layout: default
title: Git
permalink: /tutorials/git/
---
<section class="course-header">
  <h1>Git</h1>
  <p>Version control foundations, branches, collaboration, and workflows.</p>
</section>
<section class="lesson-list" aria-label="Git lessons">
{% assign lessons = site.tutorials | where: "course", "git" | sort: "order" %}
{% for lesson in lessons %}
  <a class="lesson-card" href="{{ lesson.url | relative_url }}"><span class="lesson-order">{{ lesson.order | prepend: '0' | slice: -2, 2 }}</span><span><h2>{{ lesson.title }}</h2>{% if lesson.excerpt %}<p>{{ lesson.excerpt }}</p>{% endif %}</span></a>
{% else %}
  <p class="empty-state">Lessons for this course are coming soon.</p>
{% endfor %}
</section>

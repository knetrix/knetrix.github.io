---
layout: default
title: IoT
permalink: /tutorials/iot/
---
<section class="course-header">
  <h1>IoT</h1>
  <p>ESP8266, ESP32, MQTT, sensors, Node-RED, and secure systems.</p>
</section>
<section class="lesson-list" aria-label="IoT lessons">
{% assign lessons = site.tutorials | where: "course", "iot" | sort: "order" %}
{% for lesson in lessons %}
  <a class="lesson-card" href="{{ lesson.url | relative_url }}"><span class="lesson-order">{{ lesson.order | prepend: '0' | slice: -2, 2 }}</span><span><h2>{{ lesson.title }}</h2>{% if lesson.excerpt %}<p>{{ lesson.excerpt }}</p>{% endif %}</span></a>
{% else %}
  <p class="empty-state">Lessons for this course are coming soon.</p>
{% endfor %}
</section>

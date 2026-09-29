---
layout: default
title: Blog
permalink: /blog/
---
<section class="blog-intro">
  <h1>Blog</h1>
  <p>Notes, projects, and technical writing by Knetrix.</p>
</section>
<section class="post-list" aria-label="Blog posts">
{% for post in site.posts %}
  <a class="post-card" href="{{ post.url | relative_url }}">
    <time class="post-date" datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time>
    <h2>{{ post.title }}</h2>
    {% if post.excerpt %}<p>{{ post.excerpt | strip_html | normalize_whitespace }}</p>{% endif %}
  </a>
{% else %}
  <p class="empty-state">No posts published yet.</p>
{% endfor %}
</section>

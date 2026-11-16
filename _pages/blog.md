---
layout: single
title: "Blog"
permalink: /blog/
author_profile: true
description: "Writing on conversational AI, language understanding, and machine learning research."
---
Writing on conversational AI, language understanding, and machine learning research.

<div class="post-grid">
  {% for post in site.posts %}
  <article class="post-card">
    <p class="post-card__meta">{{ post.date | date: "%d %B %Y" }} · {% include read-time.html %}</p>
    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt | strip_html | truncate: 240 }}</p>
    <a class="post-card__link" href="{{ site.baseurl }}{{ post.url }}">Read post →</a>
  </article>
  {% endfor %}
</div>

[Subscribe via RSS]({{ site.baseurl }}/feed.xml)

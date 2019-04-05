---
layout: page
title: Column
permalink: /column/
---

<div>
  {% for post in site.categories["Column"] %}
  <article class="archive-item">
    <h2><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h2>
  </article>
  {% endfor %}
</div>
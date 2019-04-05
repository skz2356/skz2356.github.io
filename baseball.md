---
layout: page
title: Baseball
permalink: /baseball/
---

<div>
  {% for post in site.categories["Baseball"] %}
  <article class="archive-item">
    <h3><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h3>
  </article>
  {% endfor %}
</div>
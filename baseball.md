---
layout: page
title: Baseball
permalink: /baseball/
---

<div>
  <div class="archive-group">
    <div id="#{{ category_name | slugize }}"></div>
    <h3 class="category-head">{{ Baseball }}</h3>
    <a name="{{ category_name | slugize }}"></a>
    {% for post in site.categories["Baseball"] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
</div>
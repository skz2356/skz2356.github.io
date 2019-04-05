---
layout: page
title: Column
permalink: /column/
---

<div>
{% for category in site.categories %}
  <div class="archive-group">
    {% capture column %}{{ category | first }}{% endcapture %}
    <div id="#{{ column | slugize }}"></div>
    <p></p>
    <h3 class="category-head">{{ Column }}</h3>
    <a name="{{ column | slugize }}"></a>
    {% for post in site.categories[column] %}
    <article class="archive-item">
      <h4><a href="{{ site.baseurl }}{{ post.url }}">{{post.title}}</a></h4>
    </article>
    {% endfor %}
  </div>
{% endfor %}
</div>
---
layout: default
---

index

{% if post.title %}
  <h1 class="entry-title">
    <a href="{{ root_url }}{{ post.url }}">{{ post.title }}</a>
  </h1>      
{% endif %}

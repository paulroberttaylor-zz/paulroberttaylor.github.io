---
layout: default
---



{% assign post = site.posts.first %}

{% for post in site.posts %}
  <div>
    <a href="{{ post.url }}">{{post.title}}</a>
  </div>
{% endfor %}



<div class="posts">
  {% for post in site.posts %}
    <article class="post">

      <h1><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></h1>

      <div class="entry">
        {{ post.excerpt }}
      </div>

      <a href="{{ site.baseurl }}{{ post.url }}" class="read-more">Read More</a>
    </article>
  {% endfor %}
</div>

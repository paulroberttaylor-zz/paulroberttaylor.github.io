---
layout: default
---

index

{% assign post = site.posts.first %}

{% for post in site.posts %}

{{post.title}}

<a href="{{ post.url }}">{{ post.url }}</a>
{% endfor %}


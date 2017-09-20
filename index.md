---
layout: default
---

index

{% assign post = site.posts.first %}

{{post.title}}

<a href="{{ post.url }}">{{ post.url }}</a>

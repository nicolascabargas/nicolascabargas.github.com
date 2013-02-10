---
layout: page
title: Falsa Modestia
tagline: by @nico_cabargas
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <li>
      <span>Publicado en {{ post.date | date_to_string }}</span> <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a>
      <hr>
      <p>{{ post.content | truncatewords: 50 }}</p>
      <hr>
      <p><a class="span2 offset4 btn btn-inverse" href="{{ BASE_PATH }}{{ post.url }}">Ver más</a><p>
    </li>
  {% endfor %}
</ul>
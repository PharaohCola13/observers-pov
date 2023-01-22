---
layout: home
title: Down to Earth
permalink: /earth
---

{% for post in paginator.posts %}
    {% if post.category == "earth" %}
  <div class="posts-container">
    <h1>
      <a href="{{ site.github.url }}{{ post.url }}">{{ post.title }}</a>
    </h1>
    {% if post.image %}
      <div class="thumbnail-container">
        <a href="{{ site.github.url }}{{ post.url }}"><img src="{{ site.github.url }}/assets/img/{{ post.image }}"></a>
      </div>
    {% endif %}
  </div>
  {% endif %}
{% endfor %}
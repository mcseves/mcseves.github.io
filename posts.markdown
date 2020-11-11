---
layout: olderposts
title: Older posts
permalink: /posts/
---

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
    <p><span><a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a></span>
        <small><span>| {{ post.date | date_to_string }}</span></small></p>
    {% endfor %}
  </ul>
{% endfor %}







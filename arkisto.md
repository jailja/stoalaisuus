---
layout: page
title: Kyykkyfilosofin päiväkirja
---

{% for tag in site.tags %}
  <h3>{{ tag[0] }}</h3>
  <ul>
    {% for post in tag[1] %}
      <li><a href="{{ post.url }}">{{ post.title }} ({{post.date | date: "%e.%m.%Y" }})</a></li>
    {% endfor %}
  </ul>
{% endfor %}
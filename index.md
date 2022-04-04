---
title: Plants
---

{% for cat in site.categories %}
  <h3>{{ cat[1][0].title }}</h3>
  <ul>
    {% for post in cat[1] %}
      <li><a href="/plants{{ post.url }}">{{ post.date | date: "%Y-%m-%d" }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

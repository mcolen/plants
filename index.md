---
title: Plants
---

{% for cat in site.categories %}
  <h3>{{ cat }}</h3>
  <ul>
    {% for post in site.categories[cat] %}
      <li><a href="{{ post.url }}">{{ post.date  | date: "%Y-%m-%d" }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

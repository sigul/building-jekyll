---
layout: default
---
<h2>Original loop for categories in Jekyll doc</h2>

{% for category in site.categories %}
  <h3>Category: {{ category[0] }}</h3>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}">{{ post.title }}</a></li>
    {% endfor %}
  </ul>
{% endfor %}

---
layout: page
permalink: pages
title: Pages stored in _pages folder
---
To be able to store pages in a folder called <code>_pages</code> you must:

1. create a folder _pages in your root
2. create pages in _pages folder and **assign permalink to each page**
3. include the folder in the _config file (<code>include: ['_pages']</code>)

----

<ul>
{% for page in site.pages %}
<li><a href="{{ page.url }}">{{ page.title }}</a></li>
{% endfor %}
</ul>

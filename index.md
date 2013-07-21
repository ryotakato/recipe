---
layout: page
---
{% include JB/setup %}

<h2>Welcome</h2>
<h4>Here is My Recipe Site</h4>

<h2>Recent Entry</h2>
<ul class="posts">
  {% for post in site.posts limit:10 %}
    <li><span>{{ post.date | date: "%Y-%m-%d" }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>



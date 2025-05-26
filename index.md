---
layout: home
title: Welcome
---

<h1>Welcome to Techn0tz blog</h1>

<!-- This code turns your homepage into a dynamic blog index. Any time you add a new post in _posts/, it automatically appears in the list — no need to manually update index.md.-->
<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ site.baseurl }}{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%B %d, %Y" }}
    </li>
  {% endfor %}
</ul>
---
title: Денис Батурин - Техноблог
---

# Денис Батурин - Техноблог  

<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

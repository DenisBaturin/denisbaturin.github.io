---
layout: default
title: Денис Батурин - Техноблог
---

# Денис Батурин - Техноблог  

  <ul class="post-list">

    {% for post in site.posts %}

      <li>

        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>

        <h2>
          <a class="post-link" href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}</a>
        </h2>

        <!-- adds post excerpt (separator set in _config.yml) -->
        {{ post.excerpt }}

        <!-- Adds read more link after post excerpt -->
        {% if post.excerpt != post.content %}
          <a href="{{ site.baseurl }}{{ post.url }}">Read more</a>
        {% endif %}

      </li>

    {% endfor %}

  </ul>

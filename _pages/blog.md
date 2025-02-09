---
permalink: /blog
layout: page
title: Blog archive
---

<ul>
  {% for post in site.posts %}
    <li>
      <h4>
        <a class="post-link" href="{{ post.url | relative_url }}">
          {{ post.title | escape }}
        </a>
      </h4>
      {% if post.tags %}
        <h5>
          Tags: {{ post.tags | join: ", " }}
        </h5>
      {% endif %}
      {%- if site.show_excerpts -%}
        {{ post.excerpt }}
      {%- endif -%}
    </li>
  {% endfor %}
</ul>

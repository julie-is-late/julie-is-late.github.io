---
permalink: /blog
layout: page
title: Blog archive
---

{% for post in site.posts %}
  <div class="post-preview">
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
      <p>{{ post.excerpt }}</p>
    {%- endif -%}
  </div>
  {% unless forloop.last %}
    <hr>
  {% endunless %}
{% endfor %}

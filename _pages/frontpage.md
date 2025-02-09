---
permalink: /
layout: home
title: Welcome
list_title: "My blog posts:"
---

{% capture resume_content %}{% include_relative resume.md %}{% endcapture %}
{{ resume_content | markdownify }}

<!--
{% capture resume_content %}{% include_relative resume.md %}{% endcapture %}
{% assign lines = resume_content | newline_to_br | split: '<br />' %}
{% assign content_lines = false %}
{% capture filtered_content %}
{% for line in lines %}
  {% if content_lines == true %}
    {{ line }}
  {% endif %}
  {% if line contains '---' %}
    {% assign content_lines = true %}
  {% endif %}
{% endfor %}
{% endcapture %}
{{ filtered_content | markdownify }}
 -->

Please check out my [github][gh] for more info!

[gh]: https://github.com/julie-is-late

---

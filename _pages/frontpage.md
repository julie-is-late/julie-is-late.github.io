---
permalink: /
layout: home
title: Welcome
list_title: "My blog posts:"
---

{% capture resume_content %}{% include_relative resume.md %}{% endcapture %}
{{ resume_content | remove: '/^---.*?---/m' | markdownify }}

Please check out my [github][gh] for more info!

[gh]: https://github.com/julie-is-late

---

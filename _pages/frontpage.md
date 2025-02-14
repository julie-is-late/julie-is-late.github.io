---
permalink: /
layout: home
title: Welcome
list_title: "My blog posts:"
---

<img src="./assets/imgs/head_shot.JPEG" width="100%">

## About

I am a systems software engineer with a focus on compilers, machine learning, and the intersection of our field with conversations around computing for good.

My nearly eight years at NVIDIA working in the Compilers Organization has allowed me to build skills that help me work independently on research-style projects. My role is focused on constructing and releasing tools which use machine learning and statistical learning methods to maximize application performance. In practice this takes many forms, but the most effective tool I have worked on focuses on applying an evolutionary search onto a search space of internal compiler optimization flags or other program runtime parameters.

Our field is one of constant change and upheaval, but I worry that as a community we are not doing enough to empower our future peers to navigate and direct this change in positive ways. I believe the only resolution to this is twofold: we need to establish a more diverse set of people in every subfield of computer science, and we need to empower STEM learners on ethical issues before they enter the field.

{% capture resume_content %}{% include_relative resume.md %}{% endcapture %}
{{ resume_content | slice: 4, resume_content.size | split: '---' | last | markdownify }}

Please check out my [github][gh] for more info!

[gh]: https://github.com/julie-is-late

---

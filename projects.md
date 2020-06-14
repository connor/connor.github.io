---
layout: default
title: Projects
permalink: /projects/
published: false
---

<div>
    {% for project in site.projects %}
        <a href="{{ project.url | prepend: site.baseurl }}">
            <h2>{{ project.title }}</h2>
        </a>
        <p class="project">{{ project.date | truncate: 160 }}</p>
    {% endfor %}
</div>

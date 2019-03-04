---
layout: page
permalink: /teaching/
title: teaching
description: Here is a list of courses and workshops I have been part of
---

<ul class="post-list">
{% for class in site.teaching reversed %}
    <li>
        <h2><a class="poem-title" href="{{ class.url | prepend: site.baseurl }}">{{ class.title }}</a></h2>
        <p class="post-meta">{{ class.date | date: '%Y' }} - {{ class.place }}</p>
      </li>
{% endfor %}
</ul>
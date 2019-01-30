---
layout: page
permalink: /publications/
title: publications
<!-- description: This is a list of publications in  -->
---

<ul class="post-list">
{% for pub in site.publications reversed %}
    <li>
        <h2><a class="poem-title" href="{{ pub.url | prepend: site.baseurl }}">{{ pub.title }}</a></h2>
        <p class="post-meta">{{ pub.date | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>
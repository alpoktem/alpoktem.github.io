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
        {% if pub.languages.size > 0 %}
        <div class="post-pills">
          {% for lang in pub.languages %}<span class="pill pill-lang">{{ lang }}</span>{% endfor %}
        </div>
        {% endif %}
        <p class="post-meta">{{ pub.date | date: '%B %-d, %Y' }}</p>
      </li>
{% endfor %}
</ul>
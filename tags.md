---
layout: default
title: Tags
---

<h1>📚 所有标签</h1>
<ul>
  {% assign tags_list = site.tags %}
  {% for tag in tags_list %}
    <li>
      <a href="/tags/{{ tag[0] | slugify }}.html">
        {{ tag[0] }} ({{ tag[1].size }})
      </a>
    </li>
  {% endfor %}
</ul>

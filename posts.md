---
layout: page
title: Posts
permalink: /posts/
---

<ul>
  {%- for post in site.posts -%}
  <li>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
    <small> — {{ post.date | date: "%b %d, %Y" }}</small>
    {%- if post.description -%}<br><em>{{ post.description }}</em>{%- endif -%}
  </li>
  {%- endfor -%}
</ul>

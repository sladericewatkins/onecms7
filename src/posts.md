---
layout: page
title: Blo(n)g(er)
---

<ul>
  {% for post in collections.posts.resources %}
    <li>
      <a href="{{ post.relative_url }}">{{ post.data.title }}</a> - posted {{ post.data.date | date_to_string: "ordinal", "US" }} by {{ post.data.author }}
    </li>
  {% endfor %}
</ul>
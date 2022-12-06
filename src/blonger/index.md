---
layout: page
title: Blo(n)g(er)
---

<ul>
  {% for post in collections.posts.resources %}
    <li>
      <a href="{{ post.relative_url }}">{{ post.data.title }}</a> - posted 📆 <b>{{ post.data.date | date_to_string: "ordinal", "US" }}</b> by ✏️ <b>{{ post.data.author }}</b>
    </li>
  {% endfor %}
</ul>
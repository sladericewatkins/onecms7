---
layout: page
title: Writing
paginate:
  collection: writing
  per_page: 12
---

This is the home for my writing. For my thoughts on things, [check out Blo(n)g(er)](https://www.sladewatkins.com/blonger/).

<ul>
  {% for post in paginator.resources %}
    <li>
      <a href="{{ post.relative_url }}">{{ post.data.title }}</a><br />Published on 📆 <b>{{ post.data.date | date_to_string: "ordinal", "US" }}</b>
    </li>
  {% endfor %}
</ul>

{% if paginator.total_pages > 1 %}
<p>Navigate:</p>
  <ul class="pagination">
    {% if paginator.previous_page %}
    <li>
      <a href="{{ paginator.previous_page_path }}">Previous Page</a>
    </li>
    {% endif %}
    {% if paginator.next_page %}
    <li>
      <a href="{{ paginator.next_page_path }}">Next Page</a>
    </li>
    {% endif %}
  </ul>
{% endif %}
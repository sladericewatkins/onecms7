---
layout: page
title: Blo(n)g(er)
paginate:
  collection: posts
  per_page: 8
---

<ul>
  {% for post in paginator.resources %}
    <li>
      <a href="{{ post.relative_url }}">{{ post.data.title }}</a><br />Posted on 📆 <b>{{ post.data.date | date_to_string: "ordinal", "US" }}</b> by ✏️ <b>{{ post.data.author }}</b>
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


Meta: <a href="https://www.sladewatkins.com/feed.xml">📰 RSS Feed (direct)</a> &bull; <a href="https://feeds.feedburner.com/sladewatkins/blonger">📰 RSS Feed (Feedburner)</a>
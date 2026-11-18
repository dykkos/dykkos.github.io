---
layout: note
title: "Mathematics"
---

Notes on combinatorics, graphs, analysis, topology, and algebra.

{% assign notes = site.pages | where: "blog_category", "Mathematics" | sort: "note_date" | reverse %}
{% if notes.size > 0 %}
<ul>
{% for note in notes %}
  <li><a href="{{ note.url | relative_url }}">{{ note.title | escape }}</a> — {{ note.note_date }}.</li>
{% endfor %}
</ul>
{% else %}
No posts yet.
{% endif %}

[All blog categories](../../blog.html).

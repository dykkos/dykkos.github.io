---
layout: note
title: "Computer Science"
---

Notes on algorithms, machine learning, systems, and programming. Project code is indexed on the [Project page](../../cs.html).

{% assign notes = site.pages | where: "blog_category", "Computer Science" | sort: "note_date" | reverse %}
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

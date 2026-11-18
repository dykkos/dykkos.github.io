---
layout: note
title: "AI Safety"
---

Personal AI-safety notes. The [TAISI reading list](../../ai-safety.html) is organized separately from these posts.

{% assign notes = site.pages | where: "blog_category", "AI Safety" | sort: "note_date" | reverse %}
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

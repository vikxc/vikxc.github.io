---
layout: default
title: Notes
---
# Notes

{% assign notes = site.notes | sort:"date" | reverse %}
<ul>
{% for note in notes %}
  <li><a href="{{ note.url }}">{{ note.title }}</a> <small style="color:#777">({{ note.date | date: "%Y-%m-%d" }})</small></li>
{% endfor %}
</ul>
<!-- Add a new Markdown file in the **notes/** folder and it will appear here. -->


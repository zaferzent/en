---
layout: page
title: Home
id: home
permalink: /
---

# Welcome! 🌱

<p style="padding: 3em 1em; background: #f5f7ff; border-radius: 4px;">
  Hello, I am Zafer. This is a place where I take notes of the things I travel, see, discover and learn. This is my first note : <span style="font-weight: bold">[[Hello World]]</span>
</p>

<strong>All notes</strong>

<ul style="padding-left: 0;">
  {% assign recent_notes = site.notes | sort: 'date' | reverse %}
  {% for note in recent_notes limit: 500 %}
    <li style="list-style-type: none; ">
      <a class="internal-link" href="{{ site.baseurl }}{{ note.url }}">{{ note.title }}</a>
    </li>
  {% endfor %}
</ul>

<style>
  .wrapper {
    max-width: 46em;
  }
</style>

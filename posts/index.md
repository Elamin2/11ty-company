---
title: Blogg
layout: layout.njk
---

# Blogg
Här är en lista över alla inlägg:
<ul>
{% for post in collections.posts %}
    <li>
        <a href="{{ post.url }}">{{ post.data.title }}</a> - <em>{{ post.data.date }}</em>
    </li>
{% endfor %}
</ul>
---
layout: default
title: Kode Snippets
permalink: /snippets/
---

<h1>Kode Snippets</h1>
<p>Her samler jeg konkrete kodeeksempler fra arbejdet i valgfaget.</p>

<ul>
{% for post in site.categories.snippets %}
  <li>
    <a href="{{ post.url }}">{{ post.title }}</a>
  </li>
{% endfor %}
</ul>

---
layout: default
title: Kode Snippets
permalink: /snippets/
---

<h1>Kode Snippets</h1>
<p>Her samler jeg kodeeksempler og screenshots fra mit arbejde.</p>

<ul class="post-list">
{% for post in site.categories.snippets %}
  <li>
    <h2><a href="{{ post.url | absolute_url }}">{{ post.title }}</a></h2>
    <p>
      <strong>Dato:</strong> {{ post.date | date: "%d-%m-%Y" }}
      {% if post.week %} &nbsp;|&nbsp; <strong>Uge:</strong> {{ post.week }}{% endif %}
    </p>
    <a href="{{ post.url | absolute_url }}">Se snippet →</a>
    <hr>
  </li>
{% endfor %}
</ul>

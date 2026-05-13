---
layout: default
title: Home
---

<header>
  <h1>Balram News</h1>
  <nav>
    <a href="#">Home</a>
    <a href="#">Politics</a>
    <a href="#">Tech</a>
    <a href="#">Sports</a>
  </nav>
</header>

<div class="container">

  {% for post in site.posts %}
  <div class="news-card">
    <h2><a href="{{ post.url }}">{{ post.title }}</a></h2>
    <p>{{ post.excerpt }}</p>
  </div>
  {% endfor %}

</div>

<footer>
  <p>© 2026 Balram News</p>
</footer>

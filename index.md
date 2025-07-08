---
layout: default
title: "Meu Blog"
---

<style>
  .home-title { font-size: 2.5rem; }
</style>

<div class="home">
  <h1 class="home-title">Olá, eu sou Isa.</h1>
  
  <p>Escrevo sobre diversas áreas que me gerarem curiosidade na computação até filosofias internas.</p>

  <h2>Posts Recentes</h2>
  <ul>
    {% for post in site.posts limit:5 %}
      <li>
        <a href="{{ post.url }}">{{ post.title }}</a> — {{ post.date | date: "%d/%m/%Y" }}
      </li>
    {% endfor %}
  </ul>
</div>
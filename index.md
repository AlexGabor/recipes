---
title: Recipes
layout: default
---

<div class="post-list">
  {% for post in site.recipes %}
  <div class="post-preview">
    <a
      href="{% if post.external %}{{ post.external_link }}{% else %}{{ post.url }}{% endif %}"
    >
      {% if post.thumbnail %}
      <div
        class="post-preview-image"
        style="background-image: url('{{ post.thumbnail }}'); background-position: center"
      ></div>
      {% endif %}

      <p class="post-preview-title">
        {% if post.external %}🔗{% endif %}{{ post.title }}
      </p>
    </a>

  </div>
  {% endfor %}
</div>

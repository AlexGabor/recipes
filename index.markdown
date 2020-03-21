---
layout: home
---
<h1>Recipes</h1>

<div class="recipe-list">
  {% for recipe in site.recipes %}
    <p class="recipe-preview">
      <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      <!-- {{ recipe.excerpt }} -->
    </p>
  {% endfor %}
</div>
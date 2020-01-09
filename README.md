# My Recipe Book

No bullshit, just vegan recipes.

<ul>
  <p>Baking</p>
  {% assign sorted_recipes = (site.pages | sort: 'title') %}
  {% for recipe in sorted_recipes %}
    {% if recipe.tags contains 'baking' %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

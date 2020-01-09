# My Recipe Book

No bullshit, just vegan recipes.

---

{% assign sorted_recipes = (recipes | sort: 'title') %}

### Baking

<ul>
  {% for recipe in sorted_recipes %}
    {% if recipe.tags contains 'baking' %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

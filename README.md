# My Recipe Book

No bullshit, just vegan recipes.

---

{% assign sorted_recipes = site.recipes | sort: 'title' %}

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

### Cooking

<ul>
  {% for recipe in sorted_recipes %}
    {% if recipe.tags contains 'cooking' %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>


### Instant Pot Friendly

<ul>
  {% for recipe in sorted_recipes %}
    {% if recipe.tags contains 'instant-pot' %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

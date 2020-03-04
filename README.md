# My Recipe Book

evolving vegan recipe book

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


### Instant Pot

<ul>
  {% for recipe in sorted_recipes %}
    {% if recipe.tags contains 'instant-pot' %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

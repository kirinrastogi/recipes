# My Recipe Book

No bullshit, just vegan recipes.

---

### Baking

<ul>
  {% for recipe in site.recipes %}
    {% if recipe.tags contains 'baking' %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

### Cooking

<ul>
  {% for recipe in site.recipes %}
    {% if recipe.tags contains 'cooking' %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>


### Instant Pot Friendly

<ul>
  {% for recipe in site.recipes %}
    {% if recipe.tags contains 'instant-pot' %}
      <li>
        <a href="{{ recipe.url }}">{{ recipe.title }}</a>
      </li>
    {% endif %}
  {% endfor %}
</ul>

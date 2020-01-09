# My Recipe Book

No bullshit, just vegan recipes.

<ul>
  {% for recipe in site.recipes %}
    <li>
      <a href="{{ recipe.url }}">{{ recipe.title }}</a>
    </li>
  {% endfor %}
</ul>

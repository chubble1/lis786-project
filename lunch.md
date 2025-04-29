---
title: Lunch
layout: page
permalink: /Lunch
image_url: https://i.ibb.co/XZ2ypRht/IMG-9638.jpg
image_alt: Image of millions of Fruit Loops.
my_variable: Lunch is served.
---
{{ page.my_variable }}

{% include page-image.html %}

A day doesn't go by that I don't look forward to lunch. Like breakfast, lunch versatility is insane, and ranges from a snack plate to a dinner-sizes entree. I love lunch!

{{ page.my_variable }}

{% for meal in site.food %}
{% if meal.category == "lunch" %}
<h3>{{ meal.title }}</h3>
<p><img src="{{ meal.image }}" alt="alt text here" /></p>
<p>{{ meal.content }}</p>
<p>Category: {{ meal.category }}</p>
{% endif %}
{% endfor %}
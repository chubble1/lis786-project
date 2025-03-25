title: Dinner
layout: page
permalink: /Dinner
image_url: 
image_alt: Image of millions of Fruit Loops.
my_variable: Dinner is served.
---
{{ page.my_variable }}
{% include page-image.html %}

This is my dinner page! Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo. Nullam dictum felis eu pede mollis pretium. Integer tincidunt.

{{ page.my_variable }}

{% for meal in site.food %}
{% if meal.category == "dinner" %}
<h3>{{ meal.title }}</h3>
<p><img src="{{ meal.image }}" alt="alt text here" /></p>
<p>{{ meal.content }}</p>
<p>Category: {{ meal.category }}</p>
{% endif %}
{% endfor %}
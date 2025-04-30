---
title: Lunch
layout: page
permalink: /Lunch
image_url: https://i.ibb.co/XZ2ypRht/IMG-9638.jpg
image_alt: Image of millions of Fruit Loops.
my_variable: Lunch is on the table.
---
{{ page.my_variable }}

A day doesn't go by that I don't look forward to lunch. Like breakfast, lunch versatility is insane, and ranges from a snack plate to a dinner-sizes entree. I love lunch!

{% include page-image.html %}

One of the best lunches I ever had was during the summer of 2016. I was 18 years old in the countryside of England, visiting an old friend's old grandmother. She took us to this pub for lunch and all three of us ordered Ploughman's Boards. Out came three wooden plates of bread, cheeses, jams, a piece of some sort of meat I'm forgetting. It was amazing. The beer was also amazing. 

From the snack plate to sandwiches \(PB&Js I love you until I'm dead\), lunch is always a wonderful time. Pictured above is a trip to Whataburger: not a vegetarian's favorite, but a true Texan knows the value of a meal shared in these beige, plastic booths. 

{{ page.my_variable }}

{% for meal in site.food %}
{% if meal.category == "lunch" %}
<h3>{{ meal.title }}</h3>
<p><img src="{{ meal.image }}" alt="alt text here" /></p>
<p>{{ meal.content }}</p>
<p>Category: {{ meal.category }}</p>
{% endif %}
{% endfor %}
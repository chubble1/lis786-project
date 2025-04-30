---
title: Breakfast
layout: page
permalink: /Breakfast
image_url: https://i.ibb.co/G3Tkvp9Q/IMG-1223.jpg
image_alt: Image of millions of Fruit Loops.
my_variable: Breakfast is ready.
---
{{ page.my_variable }}

Breakfast: the meal that begins each of our days. To some, this is a chance to fuel the body with healthy foods that improve energy and attention levels. For others, this meal is a soft and slow start to long days at the office or at home with the kids. To me, breakfast is so versatile, but when I try to prep breakfast for myself, I always come up short on ideas.

{% include page-image.html %} 

This is weird because there are so many breakfast foods I enjoy. From the Grand Slamwich at Denny's, to a 50 second microwaved poached egg, to a box of Jewel-brand Mini Wheats: I love to eat breakfast. I am also someone who usually wakes up a little hungry so I'm *ready* to eat breakfast when the time comes each morning.

Pictured above is a breakfast made by my grandma, Sue, Queen of preparing a nice meal through both taste and ambience. This particular meal was shared with my grandma *and* my mom, so it is an extra special memory for me. 

The dishes below are a diverse collection of breakfasts I've deeply enjoyed. \(However, it is possible that none of them beat eating a cold slice of leftover pizza.\)

{{ page.my_variable }}

{% for meal in site.food %}
{% if meal.category == "breakfast" %}
<h3>{{ meal.title }}</h3>
<p><img src="{{ meal.image }}" alt="alt text here" /></p>
<p>{{ meal.content }}</p>
<p>Category: {{ meal.category }}</p>
{% endif %}
{% endfor %}
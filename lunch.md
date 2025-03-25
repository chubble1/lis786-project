---
title: Lunch
layout: page
permalink: /Lunch
image_url: 
image_alt: Image of millions of Fruit Loops.
my_variable: Lunch is served.
---
{{ page.my_variable }}
{% include page-image.html %}

LUNCH! In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo. Nullam dictum felis eu pede mollis pretium. Integer tincidunt. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. 

{{ page.my_variable }}

{% for meal in site.food %}
{% if meal.category == "lunch" %}
<h3>{{ meal.title }}</h3>
<p><img src="{{ meal.image }}" alt="alt text here" /></p>
<p>{{ meal.content }}</p>
<p>Category: {{ meal.category }}</p>
{% endif %}
{% endfor %}

---
title: Breakfast
layout: page
permalink: /Breakfast
image_url: https://images.rawpixel.com/image_800/cHJpdmF0ZS9zdGF0aWMvaW1hZ2Uvd2Vic2l0ZS8yMDIyLTA0L2xyL2lzMTQ2NzEtaW1hZ2Uta3d2d3RrbmIuanBn.jpg
image_alt: Image of millions of Fruit Loops.
my_variable: Breakfast is served.
---
{{ page.my_variable }}
{% include page-image.html %}

This is my breakfast page! Gotta change something so it's gonna be this sentence... Aenean commodo ligula eget dolor. Aenean massa. Cum sociis natoque penatibus et magnis dis parturient montes, nascetur ridiculus mus. Donec quam felis, ultricies nec, pellentesque eu, pretium quis, sem. Nulla consequat massa quis enim. Donec pede justo, fringilla vel, aliquet nec, vulputate eget, arcu. In enim justo, rhoncus ut, imperdiet a, venenatis vitae, justo. Nullam dictum felis eu pede mollis pretium. Integer tincidunt.

{{ page.my_variable }}

{% for meal in site.food %}
{% if meal.category == 'breakfast' %}
<h3>{{ meal.title }}</h3>
<p><img src="{{ meal.image }}" alt="alt text here" /></p>
<p>{{ meal.content }}</p>
<p>Category: {{ meal.category }}</p>
{{% endif %}}
{% endfor %}
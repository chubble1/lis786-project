---
title: Dinner
layout: page
permalink: /Dinner
image_url: https://i.ibb.co/1tGMG86V/IMG-2158.jpg
image_alt: Image of millions of Fruit Loops.
my_variable: Dinner is served.
---
{{ page.my_variable }}

Of the three types of meals we usually eat, dinner is by far the most intimidating. It can mean so many things, be so many different dishes. I like dinner that makes me feel good about my day, despite the status of my work or scbool or relationships.

{% include page-image.html %}

Of the meals, I also spend the most time thinking about dinner: when are we eating dinner, what are we having for dinner, am I cooking dinner tonight, we should invite them over for dinner, we should make our neighbors dinner, is this dinner good for me, is this dinner good for Tanner, do the cats want to eat dinner with us, what did I forget at the store that I need in order to cook dinner?

It is a never-ending cycle of getting groceries, making dinner, cleaning dishes. Two of the three of these things I've gotten very comfortable with over the past few years. The last thing is a chore I've been begrudgingly completeing since I was a kid. When I make a nice dinner, I feel really proud. When I dress up and go eat nice food, I also feel proud. I looove discovering new dinner spots in Chicago. A lot of dishes would be on this dinner list if I had the photos to display them.  

Pictured above is a 2019 meal shared with my dear friend Scott on a trip we took to Greece together. This trip was full of cheesy dinners, roasted vegetables, spanokopita, and all good Greek drinks.

{{ page.my_variable }}

{% for meal in site.food %}
{% if meal.category == "dinner" %}
<h3>{{ meal.title }}</h3>
<p><img src="{{ meal.image }}" alt="alt text here" /></p>
<p>{{ meal.content }}</p>
<p>Category: {{ meal.category }}</p>
{% endif %}
{% endfor %}
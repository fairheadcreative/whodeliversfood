---
layout: layout
title: Directory
---
{% assign sorted = site.posts | sort: 'title' %}

<header>
  <h1><span>🚚💨</span>Who Delivers Food In The UK?</h1>
  <p>Shoot. You didn't get a slot today. That's okay, try another food delivery service!</p>
</header>

<h2>Recipe Boxes & Meal Delivery</h2>
{% for post in sorted %}
{% if post.type == "recipe" %}
<article>
  <h3><a href="{{ post.source }}">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</article>
{% endif %}
{% endfor %}

<h2>Essentials Boxes</h2>
{% for post in sorted %}
{% if post.type == "essentials" %}
<article>
  <h3><a href="{{ post.source }}">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</article>
{% endif %}
{% endfor %}

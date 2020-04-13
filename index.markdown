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
{% if post.type == "recipe" or post.type == "Recipe" %}
<article>
  <h3><a href="{{ post.source }}">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</article>
{% endif %}
{% endfor %}

<h2>Food Boxes</h2>
{% for post in sorted %}
{% if post.type == "boxes" or post.type == "Boxes" %}
<article>
  <h3><a href="{{ post.source }}">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</article>
{% endif %}
{% endfor %}

<h2>Special Eating Requirements</h2>
{% for post in sorted %}
{% if post.type == "special" or post.type == "Special" %}
<article>
  <h3><a href="{{ post.source }}">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</article>
{% endif %}
{% endfor %}

<h2>Takeaway Services</h2>
{% for post in sorted %}
{% if post.type == "takeaway" or post.type == "Takeaway"  %}
<article>
  <h3><a href="{{ post.source }}">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</article>
{% endif %}
{% endfor %}

<h2>Other</h2>
{% for post in sorted %}
{% if post.type == "other" or post.type == "Other" %}
<article>
  <h3><a href="{{ post.source }}">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</article>
{% endif %}
{% endfor %}

<h2>And what should be the sensible everyday grocery options (good luck getting a delivery slot though...)</h2>
{% for post in sorted %}
{% if post.type == "supermarkets" or post.type == "Supermarkets" %}
<article>
  <h3><a href="{{ post.source }}">{{ post.title }}</a></h3>
  <p>{{ post.description }}</p>
</article>
{% endif %}
{% endfor %}

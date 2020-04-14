---
layout: layout
title: Directory
---
{% assign sorted = site.posts | sort: 'title' %}

<header>
  <h1><span>🚚💨</span>Who Delivers Food In The UK?</h1>
  <p>Didn't get a slot today? That's okay, try another food delivery service!</p>

  <p class="detail">Thank you for being smart enough to be trying to stay at home during the global pandemic (you little wonder, you). This website is purely for your information, to help you find out where you can get food deliveries at home. To the best of our knowledge, you can get food deliveries from these companies at the moment - no guarantees though. We're just as hungry as you, and doing our best to share the options we're aware of.</p>

  <a class="twitter" href="http://twitter.com/share?text=A Directory Of Everyone Who Delivers Food In The UK:&url=https://whodeliversfood.co.uk&hashtags=covid19">Share on Twitter</a>

  <a class="facebook" href="https://www.facebook.com/sharer/sharer.php?u=https%3A//whodeliversfood.co.uk">Share on Facebook</a>

  <a class="linkedin" href="https://www.linkedin.com/shareArticle?mini=true&url=https%3A//whodeliversfood.co.uk&title=Who%20Delivers%20Food%20In%20The%20UK?&summary=A%20directory%20of%20everyone%20who%20delivers%20food%20in%20the%20UK!&source=">Share on LinkedIn</a>

  <a class="whatsapp" href="whatsapp://send?text=A Directory Of Everyone Who Delivers Food In The UK: https://whodeliversfood.co.uk" data-action="share/whatsapp/share">Share via WhatsApp</a>
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


<h2>Hints and tips</h2>
<p>Book a delivery slot before filling up your basket - especially with the supermarkets. Otherwise you'll be bitterly disappointed. (Ever had the warm, fuzzy feeling that you were soon to receive a delivery of chocolate hobnobs, only to be informed minutes later that they are NEVER COMING? Sad times, my friend).</p>
<p>When you do manage to get a delivery slot for a supermarket, be prepared for a good 50% of your order to be subbed out with totally irrational alternatives. It's a grocery lottery: sometimes you win, sometimes you get coconut and lime ice cream. Be grateful all the same, the pickers and packers are doing their best.</p>
<p>Don't buy more than you need - unless it's tins of beans. Have as many of those as you want. They keep for ages and no one else wants any more cluttering up their cupboards.</p>
<p>Wave cheerily at your delivery driver from a respectful distance to confirm receipt of your package or takeaway. You could even doff your imaginary cap in their general direction. Consider this your way of thanking them for venturing out into the big, scary world and making the journeys back and forth to keep your belly full.</p>

<article class="missed">
  <h3>Did we miss you?</h3>
  <p>If you're delivering food in England and Wales right now, and we haven't mentioned you, then <a href="mailto:hello+food@fairheadcreative.com">email us</a> or tweet <a href="https://twitter.com/adamfairhead/">@adamfairhead</a> with your details and let us know so we can add you to the list.</p>
</article>

---
layout: page
title: The world is a beautiful place
excerpt: "A few of my travels."
search_omit: true
---

<img align="center" src="/images/travel_fishwatermark.jpg" height="35%" width="35%" alt="Plitvice Lake in Croatia"/>
<p>
Plitvice lake in Croatia. The water is so pristine and blue that it looks like I went snorkeling. I'm just peering down at the lake in front it me. This was taken with an old iPhone 4S.
</p>
<br><br>
<img align="center" src="/images/travel_skullwatermark.jpg" height="35%" width="35%" alt=""/>
<p>
I visited a church made from the skeletons of monks while in Portugal.
</p>
<br><br>

<ul class="post-list">
{% for post in site.categories.travel %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

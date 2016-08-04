---
layout: page
title: The world is a beautiful place
excerpt: "A few of my travels."
search_omit: true
---


<p>
After graduating from college, I was fortunate to have been able to travel and live and work abroad. I survived the -45 degree winter in Mongolia. I resided in both 4-season and tropical parts of Vietnam. In Europe, I frequented the festivals of Bavarian Germany. My favorite home was the welcoming emerald isle of Ireland. I also visited several countries in between. Now that I'm back in the United States, New York City has proven to be just as exciting!</p>
<br><br>
Below are a couple of pictures from my travels. I'll post more when I get my media HDD fixed!
<br><br>
<img align="center" src="/images/travel_fishwatermark.jpg" height="100%" width="100%" alt="Plitvice Lake in Croatia"/>
<p>
Plitvice lake in Croatia. The water is so pristine and blue that it looks like I went snorkeling. I'm really just peering down at the lake in front of me.
</p>
<br><br>
<img align="center" src="/images/travel_skullwatermark.jpg" height="100%" width="100%" alt=""/>
<p>
While in Portugal, I visited a church made from the skeletons of monks. Eerie...
</p>
<br><br>

<ul class="post-list">
{% for post in site.categories.travel %} 
  <li><article><a href="{{ site.url }}{{ post.url }}">{{ post.title }} <span class="entry-date"><time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %d, %Y" }}</time></span>{% if post.excerpt %} <span class="excerpt">{{ post.excerpt | remove: '\[ ... \]' | remove: '\( ... \)' | markdownify | strip_html | strip_newlines | escape_once }}</span>{% endif %}</a></article></li>
{% endfor %}
</ul>

---
layout: page_resources
title:  Success Stories
subtitle: Kicking off a new collection of Success Stories.
date:   2025-04-08
categories: highlight
hero_image: /img/black.jpg
hero_height: is_fullheight
is_series: true
series_title: "Post"
---

<strong>IDEAS Watersheds is kicking off a new collection of Success Stories</strong>

[More Information](../../../../../success-stories)


<br><br> **OLDER POSTS**
{% if page.is_series == true %}
{% assign posts = site.posts | where: "is_series", true | where: "series_title", page.series_title | sort: 'date' | reverse %}

{% for post in posts %}
        {% if post.url != page.url %}
 		<a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}- {{ post.subtitle }}</a> Published on <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time><br>
        {% endif %}
{% endfor %}
{% endif %}
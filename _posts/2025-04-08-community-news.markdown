---
layout: page_resources
title:  Community News
subtitle: PFLOTRAN Webinar on Reactive Transport Models
date:   2025-04-08
categories: highlight
hero_image: /img/black.jpg
hero_height: is_fullheight
is_series: true
series_title: "Post"
---

<strong>Webinar on Building Reactive Transport Models in PFLOTRAN</strong><br>Environmental Molecular Sciences Laboratory (EMSL)<br><em>April 9th, 2025</em>

[More Information](https://www.emsl.pnnl.gov/events/emsl-learn-webinar-series-building-reactive-transport-models-pflotran-environmental?utm_campaign=April+9+PFLOTRAN+&utm_source=instagram&utm_medium=Mailchimp&utm_content=1741795956)


<br><br> **OLDER POSTS**
{% if page.is_series == true %}
{% assign posts = site.posts | where: "is_series", true | where: "series_title", page.series_title | sort: 'date' | reverse %}

{% for post in posts %}
        {% if post.url != page.url %}
 		<a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}- {{ post.subtitle }}</a> Published on <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time><br>
        {% endif %}
{% endfor %}
{% endif %}
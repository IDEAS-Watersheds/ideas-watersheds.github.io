---
layout: page_resources
title:  Community News
subtitle: ATS Short Course a big hit!
date:   2025-09-08
categories: highlight
hero_image: /img/black.jpg
hero_height: is_fullheight
is_series: true
series_title: "Post"
---

ATS Short Course a big hit!

The ATS Short Course was held September 8-10, 2025 at ORNL and the UT conference center.   It was attended by 64 people (with about 28 in person) from 4 national laboratories and 19 universities.   Attendees included senior and early-career scientists as well as students.  The complete course will be made available online through the github repository [github.com/amanzi/ats-short-course](github.com/amanzi/ats-short-course).   Input files and jupyter notebooks are there already, final slides and recordings of the lessons are coming soon.

<br><br> **OLDER POSTS**
{% if page.is_series == true %}
{% assign posts = site.posts | where: "is_series", true | where: "series_title", page.series_title | sort: 'date' | reverse %}

{% for post in posts %}
        {% if post.url != page.url %}
 		<a href="{{ post.url | prepend: site.baseurl }}">{{ post.title}}- {{post.subtitle }}</a> Published on <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time><br>
        {% endif %}
{% endfor %}
{% endif %}
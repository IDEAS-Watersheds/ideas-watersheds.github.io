---
layout: post
title:  ATS Short Course material available online
subtitle: ATS short courseATS short course
date:   2021-09-30
categories: highlight
is_series: true
series_title: "Post"
---

The first ATS short course (September 1-2, 2021) was a great success, thanks to all those who presented demos and those who
participated.  Being online we were able to attract over 50 participants from countries in Asia, Europe and North America.

The content is all available online.  The ATS short course repository
[https://github.com/amanzi/ats-short-course](https://github.com/amanzi/ats-short-course)
includes all the course material, including the slides and links to the recordings of the interactive demo sessions, which are run through Jupyter notebooks in Docker container that included Watershed Workflow and ATS.

<br><br> **OLDER POSTS**
{% if page.is_series == true %}
{% assign posts = site.posts | where: "is_series", true | where: "series_title", page.series_title | sort: 'date' | reverse %}

{% for post in posts %}
        {% if post.url != page.url %}
 		<a href="{{ post.url | prepend: site.baseurl }}">{{ post.subtitle }}</a> Published on <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time><br>
        {% endif %}
{% endfor %}
{% endif %}
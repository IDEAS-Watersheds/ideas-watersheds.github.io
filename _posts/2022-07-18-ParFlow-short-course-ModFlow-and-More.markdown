---
layout: page_resources
title:  Community News
subtitle: ParFlow Short Course at ModFlow and More
date:   2022-07-18 
categories: highlight
hero_image: /img/black.jpg
hero_height: is_fullheight
is_series: true
series_title: "Post"
---

The ParFlow Short Course titled **Integrated Simulation Of Watershed Systems Using ParFlow** was held June 2-3, 2022 at the ModFlow and More Conference.  

This class trains students in aspects of integrated hydrologic modeling using ParFlow. The course is problem based, focusing all modules and exercises on simulation of a well-studied, research watershed. Students will gain familiarity in the processes simulated with this platform, gain understanding of the disparate input and output datasets and gain understanding and familiarity of Linux commands, high performance computing, visualization and hydrologic analysis. The course is designed modularly and builds in complexity with a host of in-class exercises where the students explore this system under the guidance of the instructors.

The course material is all available online through the github repository,
[https://github.com/hydroframe/parflow_python_shortcourse](https://github.com/hydroframe/parflow_python_shortcourse). 

<br><br> **OLDER POSTS**
{% if page.is_series == true %}
{% assign posts = site.posts | where: "is_series", true | where: "series_title", page.series_title | sort: 'date' | reverse %}

{% for post in posts %}
        {% if post.url != page.url %}
 		<a href="{{ post.url | prepend: site.baseurl }}">{{ post.title}}- {{post.subtitle }}</a> Published on <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time><br>
        {% endif %}
{% endfor %}
{% endif %}
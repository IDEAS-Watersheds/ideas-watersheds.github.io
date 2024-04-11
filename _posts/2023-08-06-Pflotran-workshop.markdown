---
layout: post
title:  PFLOTRAN Reactive Transport Short Course
subtitle : PFLOTRAN Reactive Transport with Sophisticated Reaction Networks
date:   2023-08-28
categories: highlight
is_series: true
series_title: "Post"
---
A new short course, **PFLOTRAN Reactive Transport with Sophisticated Reaction Networks: Hands-On Experience with the PFLOTRAN Reaction Sandbox**, will take place Nov 6-9 at Pacific Northwest National Laboratory, Richland, WA.

Reactive transport modeling is increasingly important for solving real-world environmental issues related to water quality and ecological habitats and in evaluating the performance of environmental restoration and remediation efforts. This course will train participants in conceptualizing, implementing, and troubleshooting reaction networks in reactive transport models through hands-on experience.
  The course is a collaboration between Consortium of Universities for the Advancement of Hydrologic Science (CUAHSI) and Pacific Northwest National Laboratory and is aimed at graduate students, post-docs, professionals and senior scientists who will use reactive transport modeling as part of their work.

Registration Deadline is September 14, 2023.  Learn more and register at the CUAHSI Website, [https://www.cuahsi.org/workshops/reactive-transport-with-sophisticated-reaction-networks-hands-on-experience-with-the-pflotran-reaction-sandbox](https://www.cuahsi.org/workshops/reactive-transport-with-sophisticated-reaction-networks-hands-on-experience-with-the-pflotran-reaction-sandbox).

<br><br> **OLDER POSTS**
{% if page.is_series == true %}
{% assign posts = site.posts | where: "is_series", true | where: "series_title", page.series_title | sort: 'date' | reverse %}

{% for post in posts %}
        {% if post.url != page.url %}
    <a href="{{ post.url | prepend: site.baseurl }}">{{ post.subtitle }}</a> Published on <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time><br>
        {% endif %}
{% endfor %}
{% endif %}
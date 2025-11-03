---
layout: page_resources
title:  Community News
subtitle: Congratulations to Laura Condon!
date:   2025-09-25
categories: highlight
hero_image: /img/black.jpg
hero_height: is_fullheight
is_series: true
series_title: "Post"
---

<strong>Congratulations to Laura Condon</strong>, our IHSI co-lead, for winning the prestigious <em>Macelwane Medal</em> from the American Geophysical Union!

<style>
    .cont {
      display: flex;
      flex-wrap: wrap;
    }

.col1 {
      flex: 3; 
      min-width: 200px;
      padding-top: 20px;
      padding-right: 20px;
    }

.col2 {
      flex: 1;
      min-width: 200px;
      padding-top: 20px;
    }

</style>

<body>
    <div class="cont">
      <div class="col1">
        <p>In IDEAS-Watersheds Laura co-leads the Integrated Hydrologic Simulation Infrastructure (IHSI) activity, which is builds on the theme of her broader research that strives to reshape how scientists view groundwater’s role in the hydrologic cycle and its critical connection to climate, ecosystems, and human water use.  The James B. Macelwane Medal is awarded to early career scientists nominated on the breadth of their research, impact, creativity as well as service and community outreach.  Laura has made contributions in all these areas, contributing at the highest levels such as the National Climate Assessment and advised the White House President’s Council of Advisors on Science and Technology on groundwater issues, and at the grass roots level through teaching and the development of open-source software and FAIR data sets for open science. </p>
        <p>Here is the  <a href="https://has.arizona.edu/news/updated-congratulations-has-professor-laura-condon-2025-recipient-agus-james-b-macelwane-medal">link to the full story</a> from the University of Arizona</p>
      </div>
        <div class="col2">
            <img src="/img/photos/lcondon2.png" align="center"><br>
        </div>
    </div>
</body>




<br><br> **OLDER POSTS**
{% if page.is_series == true %}
{% assign posts = site.posts | where: "is_series", true | where: "series_title", page.series_title | sort: 'date' | reverse %}

{% for post in posts %}
        {% if post.url != page.url %}
 		<a href="{{ post.url | prepend: site.baseurl }}">{{ post.title }}- {{ post.subtitle }}</a> Published on <time datetime="{{ post.date | date_to_xmlschema }}">{{ post.date | date: "%B %-d, %Y" }}</time><br>
        {% endif %}
{% endfor %}
{% endif %}
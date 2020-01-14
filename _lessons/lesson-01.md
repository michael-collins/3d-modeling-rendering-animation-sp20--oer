---
title: Lesson 01
subtitle: 3D modeling
layout: lesson
learning objectives:
---

###Presentation

###Topics
<ul>
 {% for topic in site.topics %}
   {% for tag in topic.tags %}
       {% if tag == "maya-modeling" %}
           <li><a href="{{ topic.url | prepend: site.baseurl }}">{{topic.title}}</a></li>
        {% endif %}
   {% endfor %}
 {% endfor %}
</ul>

###Exercise

####<a href="/3d-digital-art-and-design--oer/exercises/maya-image-planes-for-modeling/maya-image-planes-for-modeling.html"><span class="exercise-title">Maya Image Planes for Modeling</span></a>

####<a href="/3d-digital-art-and-design--oer/exercises/maya-modeling/maya-modeling.html"><span class="exercise-title">Modeling</span></a>

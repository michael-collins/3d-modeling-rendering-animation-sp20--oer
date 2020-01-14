---
title: Lesson 03
subtitle: Lighting and rendering
layout: lesson
---

###Topics
<ul>
 {% for topic in site.topics %}
   {% for tag in topic.tags %}
       {% if tag == "maya-lighting-rendering" %}
           <li><a href="{{ topic.url | prepend: site.baseurl }}">{{topic.title}}</a></li>
        {% endif %}
   {% endfor %}
 {% endfor %}
</ul>

###Exercise

####<a href="/3d-digital-art-and-design--oer/exercises/maya-layered-shaders/maya-layered-shaders.html"><span class="exercise-title">Maya Layered Shaders</span></a>

####<a href="/3d-digital-art-and-design--oer/exercises/maya-mentalray-lighting-and-rendering/maya-mentalray-lighting-and-rendering.html"><span class="exercise-title">MentalRay</span></a>

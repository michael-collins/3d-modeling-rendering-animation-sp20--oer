---
title: Lesson 02
subtitle: Texturing
layout: lesson
---

###Topics
<ul>
 {% for topic in site.topics %}
   {% for tag in topic.tags %}
       {% if tag == "maya-texturing" %}
           <li><a href="{{ topic.url | prepend: site.baseurl }}">{{topic.title}}</a></li>
        {% endif %}
   {% endfor %}
 {% endfor %}
</ul>

###Exercise
 
####<a href="/3d-digital-art-and-design--oer/exercises/maya-texturing/maya-texturing.html"><span class="exercise-title">Maya Texturing</span></a>
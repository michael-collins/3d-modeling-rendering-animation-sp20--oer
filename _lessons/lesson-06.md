---
title: Lesson 06
subtitle: Animating
layout: lesson
---

###Topics
<ul>
 {% for topic in site.topics %}
   {% for tag in topic.tags %}
       {% if tag == "maya-animation" %}
           <li><a href="{{ topic.url | prepend: site.baseurl }}">{{topic.title}}</a></li>
        {% endif %}
   {% endfor %}
 {% endfor %}
</ul>

###Exercise

####<a href="/3d-digital-art-and-design--oer/exercises/maya-animation/maya-animation.html"><span class="exercise-title">Maya Animation</span></a>

####<a href="/3d-digital-art-and-design--oer/exercises/maya-animated-textures/maya-animated-textures.html"><span class="exercise-title">Maya Animated Textures</span></a>
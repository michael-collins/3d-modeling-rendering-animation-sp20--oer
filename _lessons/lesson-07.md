---
title: Lesson 07
subtitle: Dynamics and simulation
layout: lesson
---

###Topics
<ul>
 {% for topic in site.topics %}
   {% for tag in topic.tags %}
       {% if tag == "maya-dynamics" %}
           <li><a href="{{ topic.url | prepend: site.baseurl }}">{{topic.title}}</a></li>
        {% endif %}
   {% endfor %}
 {% endfor %}
</ul>

###Exercise

####<a href="/3d-digital-art-and-design--oer/exercises/maya-image-planes-for-modeling/maya-image-planes-for-modeling.html"><span class="exercise-title"> Maya Image Planes for Modeling</span></a>

         - exercise : maya-dynamics
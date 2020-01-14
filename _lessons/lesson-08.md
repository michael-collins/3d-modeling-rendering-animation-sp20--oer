---
title: Lesson 08
subtitle: Compositing
layout: lesson
---

###Topics
<ul>
 {% for topic in site.topics %}
   {% for tag in topic.tags %}
       {% if tag == "maya-compositing" %}
           <li><a href="{{ topic.url | prepend: site.baseurl }}">{{topic.title}}</a></li>
        {% endif %}
   {% endfor %}
 {% endfor %}
</ul>

###Exercise

####<a href="/3d-digital-art-and-design--oer/exercises/maya-render-passes-in-mentalray/maya-render-passes-in-mentalray.html"><span class="exercise-title">Render Passes</span></a>
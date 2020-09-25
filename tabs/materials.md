---
title: Relevant Materials
---

{% for m in site.data.materials %}
{% if m.type == 'video' %}
<div class="video">
    <h1>{{ m.title }}</h1>
    <iframe width="560" height="315" src="https://www.youtube.com/embed/{{ m.video-id }}" 
    frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; 
    gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
{% endif %}
{% endfor %}

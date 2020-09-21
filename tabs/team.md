---
title: Team
---

> This is a collaborative project between Texas Tech University and the University of Southern California

{% for m in site.data.team %}
<div class="team">
    <div class="team-photo">
        <img src="/assets/img/{{ m.photo }}"/>
    </div>
    <div class="team-info">
        <h1>{{ m.name }}</h1>
        <div>
            <span>{{ m.role }}</span><br/>
            <span style="color: #666">{{ m.institution }}</span>
        </div>
    </div>
</div>
{% endfor %}

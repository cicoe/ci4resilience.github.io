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
        <h1>{% if m.website.size > 0 %}<a href="{{ m.website }}" target="_blank">{% endif %}{{ m.name }}{% if m.website.size > 0 %}</a>{% endif %}</h1>
        <div>
            <span style="color: #666">{{ m.institution }}</span><br/>
            <span>{{ m.role }}&nbsp;</span><br/>
        </div>
    </div>
</div>
{% endfor %}

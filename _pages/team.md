---
layout: archive
title: "Team"
permalink: /team/
author_profile: true
---

<div class="team-members">
    {% for member in site.team %}
        <div class="team-member" style="display: inline-block; width: 33.33%; padding: 10px;">
            <a href="{{ member.url }}" target="_blank" rel="noopener noreferrer">
                <img src="{{ member.image }}" alt="{{ member.name }}" style="border-radius: 50%; width: 100px;">
                <h2 style="font-size: 18px;">{{ member.name }}</h2>
                <p style="font-size: 14px;">{{ member.affiliation }}</p>
            </a>
        </div>
        {% if forloop.index0|divisibleby:3 and forloop.index0 != 0 %}
            <div style="clear: both;"></div>
        {% endif %}
    {% endfor %}
</div>

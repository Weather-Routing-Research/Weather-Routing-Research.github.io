---
layout: default
title: "Team"
permalink: /team/
author_profile: true
---

<div class="team-members">
    {% for member in site.team %}
        <div class="team-member">
            <a href="{{ member.url }}">
                <img src="{{ member.image }}" alt="{{ member.name }}" style="border-radius: 50%; width: 100px;">
                <h2>{{ member.name }}</h2>
                <p>{{ member.affiliation }}</p>
            </a>
        </div>
    {% endfor %}
</div>

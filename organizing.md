---
layout: page
permalink: /organizing/
title: Organizing
---

<h2 class="section-header">Organizers</h2>
<div class="team-wrapper">
    {% for team in site.data.organizing %}
    <h4 class="section-header">{{ team.name }}</h4>
    <div class="organizers-wrapper">
    {% for member in team.members %}
        <p><span class="amb-name">{{ member.name }}</span>, {{ member.affiliation }}</p>
    {% endfor %}
    </div>
    {% endfor %}
</div>

<h2 class="section-header">Ambassadors</h2>
<div class="ambassadors-wrapper">
    {% for amb in site.data.ambassadors %}
        <p><span class="amb-name">{{ amb.name }}</span>, {{ amb.affiliation }}</p>
    {% endfor %}
</div>
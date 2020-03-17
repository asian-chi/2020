---
layout: about
title: Program
permalink: /program/
---

<div class="abstract">
    <h2>Date & Venue</h2>
    <div class="abstract-overview">
        <ul class="sidebar-items program">
            <li>Date: April 25, 2020 (Saturday)</li>
            <li>Time: 09:00 - 17:00</li>
            <li>Venue: Hawai'i Convention Center, Honolulu, Hawai'i, USA</li>
        </ul>
    </div>
    <h2>Schedule</h2>
    {% if site.data.program.size > 0 %}
    <ul class="sidebar-items program">
        {% for item in site.data.program %}
            <li>
                <p>
                    <span class="news-date">{{ item.time }}</span> &#187; 
                    <span class="news-text">{{ item.activity }}</span>&nbsp;
                    {% if item.speaker %}
                        <a class="program-speaker" href="{{ item.website }}" target="_blank">{{ item.speaker }}</a>,
                        {{ item.affiliation }} | <a href="{{ item.link }}">Bio & Abstract</a>
                    {% endif %}
                    {% if item.groups %}
                        <ul class="sidebar-items program group">
                            {% for group in item.groups %}
                            <li>
                                <p>
                                    <span class="news-date">{{ group.time }}</span> &#187; 
                                    <span class="news-text">{{ group.activity }}</span>
                                </p>
                            </li>
                            {% endfor %}
                        </ul>
                    {% endif %}
                </p>
                {% if item.note %}<p class="program-note">{{ item.note }}</p>{% endif %}
            </li>
        {% endfor %}
    </ul>
    {% endif %}
    <h2>Keynote Speakers</h2>
    <div class="abstract-overview">
        <ul class="sidebar-items keynote">
            {% for item in site.data.keynote %}
                <li>
                    <img class="keynote-photo" src="../{{ item.photo }}"/>
                    <a class="keynote-speaker" href="{{ item.website }}" target="_blank">{{ item.name }}</a>
                    {{ item.affiliation }}
                </li>
            {% endfor %}
        </ul>
    </div>
    <h2 id="accepted-submissions">Accepted Submissions</h2>
    {% if site.data.accepted.size > 0 %}
    <ul class="sidebar-items program">
        {% for item in site.data.accepted %}
            <li class="accepted-submission">
                <div class="accepted-id">#{{ item.num }}</div>
                <div class="accepted-details">
                    {% if item.type %}
                    <span class="accepted-type">{{ item.type }}</span>
                    {% endif %}
                    <span class="accepted-title">{{ item.title }}</span>
                    <p class="accepted-authors">{{ item.authors }}</p>
                    <p class="accepted-abstract">{{ item.abstract }}</p>
                </div>
            </li>
        {% endfor %}
    </ul>
    {% endif %}
</div>
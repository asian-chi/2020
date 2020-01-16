---
layout: main
---

<div class="abstract">
    <div class="banner">
        <div class="latest-symposium">
            <h4>Aloha!</h4>
            <p>The 2020 edition will take place at the Hawai'i Convention Center on the beautiful island of Oahu, Hawaiʻi, USA.</p>
        </div>
    </div>
    <p class="abstract-overview">
        The Asian CHI Symposium showcases the latest HCI work from <span class="about-highlight">Asia, the Asian diaspora and those focusing on incorporating Asian sociocultural factors in their design and implementation</span>. Aside from circulating ideas, identifying emerging research problems and envisioning future directions in human-computer interaction research, this symposium aims to foster social ties among academics (researchers and students) and practitioners and continuously grow a research community in Asia.
    </p>
    <p class="abstract-overview">
        At <a href="https://chi2020.acm.org" target="_blank">CHI 2020</a>, we plan to continue the successes of the 2019 edition by bringing together more research leaders from Asia and the Asian daspora. Specifically, we encourage participation from the other underrepresented regions of Middle East and South Asia.
    </p>
    <h4>Keynote Speakers</h4>
    {% if site.data.keynote.size > 0 %}
    <ul class="sidebar-items">
        {% for item in site.data.keynote %}
            <li>
                <p><span class="news-date">{{ item.date }}</span> &#187; <span class="news-text">{{ item.text }}</span></p>
            </li>
        {% endfor %}
    </ul>
    {% else %}
    <p>In past editions, the symposium has invited a diverse and excellent line up of keynote speakers. We will announce the 2020 line up as they confirm.</p>
    {% endif %}
    <!-- <h4>"Honu"</h4>
    <p>
        The 2020 symposium uses a Hawaiian Green Sea Turtle or "Honu" in its logo to symbolize the renewed goals of the symposium. Leading up to CHI 2021 in Asia, we aim to use the symposium as an avenue to identify promising work and help them in writing their future submissions. 
    </p> -->
</div>

<div class="news-sidebar">
    <h4>Important Dates</h4>
    <ul class="sidebar-items">
        {% for item in site.data.dates %}
            {% if item.round %}
            <p class="round-name">{{ item.round }}</p>
            {% for date in item.dates %}
            <li class="round-date">
                <p class="news-text">{{ date.text }}:</p>
                <p class="news-date">{{ date.date }}{% if date.time %} at <a href="{{ item.timezone }}" target="_blank">{{ date.time }}</a> {% endif %}</p>
            </li>
            {% endfor %}
            {% else %}
            <li>
                <p class="news-text">{{ item.text }}:</p>
                <p class="news-date">{{ item.date }}{% if item.time %} at <a href="{{ item.timezone }}" target="_blank">{{ item.time }}</a> {% endif %}</p>
            </li>
            {% endif %}
        {% endfor %}
    </ul>
    <br>
    <a class="cta-btn" href="https://asianchi20.hotcrp.com/" target="_blank">Make a Submission</a>
</div>

> Photo by <a href="https://unsplash.com/@jarvisphoto?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText" target="_blank">Braden Jarvis</a> on <a href="https://unsplash.com">Unsplash</a>.
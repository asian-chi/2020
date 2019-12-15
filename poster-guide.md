---
layout: about
title: Guide for Posters
permalink: /poster-guide/
---

<div class="abstract">
    <h2>Purpose and Design</h2>
    <div class="abstract-overview">
        <p>
            Imagine a large conference hall with 50+ posters lined up. Conference attendees will spend 5–10 seconds glancing at each poster from 1–2 meters distance before moving closer to the poster that they are interested in. Another signal that they will look for is the number of people who are currently checking out the poster and talking to the author. Once they decided that they are interested in your poster, they will move closer and start reading the title of your poster.
        </p>
        <p>
            Therefore, <span class="about-highlight">the main job of your poster is to draw the conference attendee in</span>. You should use one prominent image in your poster to achieve this. This main image should either show the uniqueness of your project (e.g., a cool photo of novel hardware or a screenshot that looks different than typical applications) or show the application domain that your project benefits from (e.g., showing the user performing a task). In either case, the main figure need to make your poster stand out from other posters. This uniqueness should be discernible from other posters at two meters distance.
        </p>
        <p>
            Once you get the attendees to look closer at your poster, the rest of the poster should <span class="about-highlight">aid your conversation with the audience</span>. Since you will be presenting your poster, verbal information should be communicated to your audience primarily from you. Therefore, the poster should provide visual aid that you will use during this conversation. Such aids may include the following:
        </p>
        <ul>
            <li>Schematics or diagrams (simplified, if need be)</li>
            <li>Image showing details of your project</li>
            <li>Charts showing main results</li>
        </ul>
        <p>
            Since these visual elements will be used when your audience stands closer to the poster, they can be much smaller, readable within 0.5 meter distance. In some projects, you may be able to incorporate some of these elements into the main image such that it can be first attractive and then provide details when look closer.
        </p>
        <p>
            While you present the poster, there may be some attendees who came in after you started talking to a few people. Thus, the poster should <span class="about-highlight">help people who visit in the middle of your conversation to catch up</span>. This can be achieved by <span class="about-highlight">an economical use of text on the following elements</span>:
        </p>
        <ul>
            <li>Title and subtitle</li>
            <li>Major talking points (1–3 sentences each): Research question and description of the work (e.g., composition of the artifact or method of study)</li>
            <li>Results</li>
            <li>Benefit of your work</li>
        </ul>
        <p>
            The <span class="about-highlight">last purpose of your poster is being a stand-in for your verbal presentation</span>. Therefore, you should <span class="about-highlight">never write long paragraphs</span> on your poster. If you are not around your poster, the poster should give enough information to tease the audience to read your work in detail.
        </p>
        <p>
            You should provide a <span class="about-highlight">convenient pointer for the audience to look up your paper</span>. Therefore, you should include the following:
        </p>
        <ul>
            <li>URL to your project. If your URL is long, use a URL shortening service, e.g., tinyurl.com/short-project-name.</li>
            <li>A QR code corresponding to the URL.</li>
        </ul>
        <p>
            Keep in mind that not everyone will carry a device with QR code reader. Short, human-readable URL should always be present
        </p>
        <p>
            Lastly, put affiliation logos on your poster. The placement of these logos should not compete with important elements of your poster (especially title and URL). Here are some example placements:  
        </p>
        <ul>
            <li>Place the logos at the very top, with an explicit visual boundary (space or color region) from your title. Imagine cutting this region off, your poster title should still be intact. Avoid this style if you have more than two logos because they clutter really quick.</li>
            <li>Place the logos at the bottom-right corner and project URL at the bottom-left corner. Leave an ample blank space in the middle.</li>
        </ul>
    </div>
</div>

<div class="news-sidebar">
    <h4>Important Dates</h4>
    <ul class="sidebar-items">
        {% for item in site.data.dates %}
            <li>
                <p class="news-text">{{ item.text }}:</p>
                <p class="news-date">{{ item.date }}{% if item.time %} at <a href="{{ item.timezone }}" target="_blank">{{ item.time }}</a> {% endif %}</p>
            </li>
        {% endfor %}
    </ul>
    <h4>Submission Details</h4>
    <ul class="sidebar-items">
        <li>Online Submission: PCS 2.0 Submission <em>(link to follow)</em></li>
        <li>Template: <a href="https://chi2020.acm.org/authors/chi-proceedings-format/" target="_blank">CHI 2020 Proceedings Format</a></li>
    </ul>
</div>
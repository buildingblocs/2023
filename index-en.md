---
layout: default
published: true
permalink: /
lang: en
---

<section class="jumbo">
    <div class="main-div">
        <h1>{{ site.title }}</h1>
        <h1><span class="huge">2023</span></h1>
        <!-- <h4>Thursday 2 June - Saturday 4 June</h4> -->
        <!-- <h4>NUS School of Computing / Online</h4> -->
	    <!-- <h4><a class="btn" href="{{ site.baseurl }}/events/june-conference/">Find Out More!</a></h4> -->
	    <h3> Scroll down for more info! </h3>
    </div>
</section>
<br><br><br>


This year, our conference is divided into two **different** events, focused on **different** themes altogether. These are the March and June Conferences!

## The March Conference

The March Conference aims to foster an interest in programming in general, and we do this by introducing participants to various programming languages, such as Python and JavaScript, and also some Markup Formats (notably HTML/CSS).

The introductory concepts introduced in these workshops function as a "first-step" for BuildingBloCS before we move on to bigger and higher-level events.

Capping off the March Conference will be a contest, but one that might catch some off guard. Unlike the classic Hackathon adopted in the June Conference, we will instead be taking inspiration from Google Summer of Code and Hacktoberfest, organising our very own "Hackathon" for open-source!

More details will be released shortly.


## The June Conference

Our flagship event of the year, the June Conference will be held in around the first week of June, with a central theme: **Artificial Intelligence (AI)**. We'll focus on the integration of AI into numerous fields, like Health, the Government and Industry, and we're also proud to partner with <a href="https://aisingapore.org/">AI Singapore</a> again!


 <!-- in their new <a href="https://aisingapore.org/student-outreach-programme/">AI Student Outreach Programme</a> which encourages students to form Student User Groups (SUG) to promote AI literacy and experiment with our open-source AI tools ‘AI BRICKS’ to develop solutions for their schools and real-world needs. -->

<!-- With the increasing importance of Computing education and AI literacy globally as well as disruptive emerging blockchain technologies, this year's focus areas will be on Computational Thinking, Artificial Intelligence and Blockchain Education! -->

<!-- We are proud to partner with <a href="https://aisingapore.org/">AI Singapore</a> again in their new <a href="https://aisingapore.org/student-outreach-programme/">AI Student Outreach Programme</a> which encourages students to form Student User Groups (SUG) to promote AI literacy and experiment with our open-source AI tools ‘AI BRICKS’ to develop solutions for their schools and real-world needs.

Learn about <a href="https://www.youtube.com/watch?v=KI3INCiyst8&t=905s">Introduction to Blockchain</a> and <a href="https://www.youtube.com/watch?v=kde1nxLN43w&t=382s">Introduction to NFTs</a> by <a href="https://www.tzapac.com/">TZAPAC</a>, official industry partner of <a href="https://noisg.comp.nus.edu.sg/noi/">National Olympiad in Informatics 2023</a>. -->

<!-- ## Schedule

This year, BuildingBloCS' main June Conference will be held over 3 days in a hybrid manner! Please refer to the schedule below for more details:

{% for day in site.data.schedule %}
{% if site.data.schedule.size > 1 %}<h2>Day {{ day.day }}</h2>{% endif %}
<table width="80%">
    {% for activity in day.activities %}
    <tr>
        <td>{{ activity.time }}</td>
        <td width="80%">{{ activity.title }}</td>
    </tr>
    {% endfor %}
</table>
{% endfor %} -->

## Organisers

<section class="organisers">
    {% for organiser in site.data.organisers %}
    <a href="{{ organiser.url }}">
        <img src="{{ site.baseurl }}/assets/img/{{ organiser.img }}" title="{{ organiser.title }}" />
    </a>
    {% endfor %}
</section>

## Partners

<section class="organisers">
    {% for partner in site.data.partners %}
    <a href="{{ partner.url }}">
        <img src="{{ site.baseurl }}/assets/img/{{ partner.img }}" title="{{ partner.title }}" />
    </a>
    {% endfor %}
</section>

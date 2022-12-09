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

The March Conference aims to foster an interest in programming in general, and we do this by introducing participants to 
various programming languages, such as Python and JavaScript, and also some Markup Formats (notably HTML/CSS).

The introductory concepts introduced in these workshops function as a "first-step" for BuildingBloCS before we move on to 
bigger and higher-level events.

Capping off the March Conference will be a contest, but one that might catch some off guard. Unlike the classic Hackathon 
adopted in the June Conference, we will instead be taking inspiration from [Hacktoberfest](https://hacktoberfest.com/)
and [Google Summer of Code](https://summerofcode.withgoogle.com/) by organising our very own "Hackathon" for open-source!

More details will be released shortly.




## The June Conference

Our flagship event of the year, the June Conference will be held in around the first week of June, with a central theme: 
**Artificial Intelligence (AI)**. We'll focus on the integration of AI into numerous fields, like Health, the Government 
and Industry, and we're also proud to partner with <a href="https://aisingapore.org/">AI Singapore</a> again!


## Organising Schools

<section class="organisers">
    {% for school in site.data.schools %}
    <a href="{{ school.url }}">
        <img src="{{ site.baseurl }}/assets/img/{{ school.img }}" title="{{ school.title }}" />
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

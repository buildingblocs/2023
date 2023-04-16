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
	    <h3>Our June Conference is out!</h3>
    </div>
</section>
<br><br><br>


This year, our conference is divided into three **different** events, focused on **different** themes altogether. These are the June, March and FOSSASIA Conferences!

## The June Conference
Our flagship event of the year, the June Conference will be held in around the first week of June, with a central theme: **Artificial Intelligence (AI)**. We're hosting over 17 workshops, 5 talks and 3 hackathons for programmers of various skill levels from beginner to advanced, and we're also proud to partner with Meta, CYS and AISG! <a href="{{ site.baseurl }}/events/june-conference">Learn more</a> and <a href="https://go.buildingblocs.sg/june">sign up</a> now!

## The March Conference
The March Conference aims to foster an interest in programming in general. We did this in March 2023 by introducing participants to various programming languages, such as Python and JavaScript, and also hosting our own Python-based beginner gamified competition! Learn more <a href="{{ site.baseurl }}/events/march-conference">here</a>!

## FOSSASIA OpenTechSummit Singapore
We held a series of workshops and connected with industry professionals at FOSSASIA 2023, held from April 13 to April 15 this year! Learn more <a href="fossasia">here</a>. 


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

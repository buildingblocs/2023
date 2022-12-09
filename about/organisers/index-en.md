---
layout: default
published: true
permalink: about/organisers/
lang: en
---

<style>
    h1, div, p {
        margin: 0px;
        padding: 0px;
    }
    a{
        text-decoration: none;
        color: inherit;
    }
    .cover{
        height: 120px;
        width: 100%;
        background: #FF9900;
        position: absolute;
        left: 0px;
        top: 0px;
        border-top-left-radius: 5px;
        border-top-right-radius: 5px;
    }
    .card {
        position: relative;
        display: inline-block;
        background: #ffffff;
        border-radius: 5px;
        box-shadow:  0 12px 13px rgba(0,0,0,0.16), 0 12px 13px rgba(0,0,0,0.16);
        text-align: center;
        padding: 20px;
        margin: 5px;
        padding-top: 5px;
        transition: all 0.5s;
    }
    .card .fa-github {
        position: absolute;
        color: #646464;
        font-size: 20px;
        top: 10px;
        right: 10px;
    }
    .card .card-title {
        color: #434343;
        margin-bottom: -8px;
        font-size: 25px;
        font-weight: 600;
    }
    .card .card-responsename {
        margin-bottom: 20px;
        color: #797979;
    }
    .card .card-desc {
        font-weight: 500;
        width: 240px;
        margin: auto;
        display: block;
        color: #3c3c3c;
        height: 120px;
    }
    .card .card-img-wrapper {
        position: relative;
        height: 160px;
        width: 160px;
        margin: 10px auto;
        margin-bottom: 20px;
    }
    .card .card-img-wrapper img {
        height: 100%;
        width: 100%;
        border-radius: 50%;
    }
    .card .card-footer {
        margin-top: 40px;
    }
    .card .card-footer .footer-box {
        position: relative;
        border-top: 2px solid #FF9900;
        box-shadow: 0 3px 6px -1px rgb(0 0 0 / 26%), 0 2px 4px -1px rgb(0 0 0 / 6%);
        border-radius: 5px;
        margin: 0 auto;
        padding: 10px;
        display: flex;
        justify-content: space-around;
    }
    .card .card-footer .footer-box .box-wrapper {
        position: relative;
    }
    .card .card-footer .footer-box .box-wrapper .count {
        font-family: 'consolas'
        color: #434343;
        font-size: 20px;
        font-weight: 600;
    }
    .card .card-footer .footer-box .box-wrapper .box-text {
        font-size: 12px;
        font-weight: 600;
        color: #00000085;
        letter-spacing: 0.5px;
    }
</style>

# Our Team

<h2 style="text-align:left;">Our OICs</h2>

BuildingBloCS 2023 is led by a set of ~~charismatic~~ passionate overall ICs who overlook various departments within the organisation. Having worked together on organising BuildingBloCS 2022 last year, the organisers
aim to help make BuildingBloCS 2023 even bigger and more far-reaching than ever before.


<section>
    {% for organiser in site.data.oics %}

    <div class="card">
        <div class="cover"></div>
        <div class="card-wrapper">
            <div class="card-header">
                <div class="card-img-wrapper">
                    <img src="{{ site.baseurl }}/assets/img/{{ organiser.img }}" width="400px" />
                </div>
                <h1 class="card-title">{{ organiser.name }}</h1>
                <div class="card-responsename"><a href="https://github.com/{{ organiser.github }}" target="_blank" rel="noopener">@{{ organiser.github }}</a></div>
                {% if organiser.bio %}
                    <p class="card-desc">{{ organiser.bio }}</p>
                {% else %}
                    <p class="card-desc">{{ organiser.level }} Student at {{ organiser.school }}</p>
                {% endif %}
                <div class="card-footer">
                    <div class="footer-box">
                        {% for comm in organiser.comms %}
                        <div class="box-wrapper">
                            <div class="count">{{ comm }}</div>
                        </div>
                        {% endfor %}
                    </div>
                </div>
            </div>
        </div>
    </div>

    {% endfor %}
</section>


<h2 style="text-align:left;">Our Organisers</h2>

Without our organizers, we wouldn't be able to organize much of BuildingBloCS, hence this serves as a _thank-you note_ to all of them for their willingness to help and make BuildingBloCS possible!

<section>
    {% for organiser in site.data.organisers %}

    <div class="card">
        <div class="cover"></div>
        <div class="card-wrapper">
            <div class="card-header">
                <div class="card-img-wrapper">
                    <img src="{{ site.baseurl }}/assets/img/{{ organiser.img }}" width="400px" />
                </div>
                <h1 class="card-title">{{ organiser.name }}</h1>
                <div class="card-responsename"><a href="https://github.com/{{ organiser.github }}" target="_blank" rel="noopener">@{{ organiser.nickname | default: organiser.github }}</a></div>
                {% if organiser.bio %}
                    <p class="card-desc">{{ organiser.bio }}</p>
                {% else %}
                    <p class="card-desc">{{ organiser.level }} Student at {{ organiser.school }}</p>
                {% endif %}
                <div class="card-footer">
                    <div class="footer-box">
                        {% for comm in organiser.comms %}
                        <div class="box-wrapper">
                            <div class="count">{{ comm }}</div>
                        </div>
                        {% endfor %}
                    </div>
                </div>
            </div>
        </div>
    </div>

    {% endfor %}
</section>

<h2 style="text-align:left;">Teachers-in-Charge</h2>

<section align="center">
    <div class="card">
        <div class="cover"></div>
        <div class="card-wrapper">
            <div class="card-header">
                <div class="card-img-wrapper">
                    <img src="{{ site.baseurl }}/assets/img/gipeh.png" width="400px" />
                </div>
                <h1 class="card-title">Mr Gi Soong Chee</h1>
                <div class="card-responsename"><a href="https://github.com/dhsgisc" target="_blank" rel="noopener">@dhsgisc</a></div>
                <p class="card-desc"><i>Make it harder.</i></p>
            </div>
        </div>
    </div>
</section>

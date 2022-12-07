---
layout: default
published: true
permalink: about/organisers/
lang: en
---

# Our Organisers


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
        background: #FF5C5C;
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
    .card .card-title {
        color: #434343;
        margin-bottom: 5px;
        font-size: 20px;
        font-weight: 600;
    }
    .card .card-desc {
        font-weight: 500;
        width: 250px;
        margin: auto;
        display: block;
        color: #3c3c3c;
    }
    .card .card-img-wrapper {
        position: relative;
        height: 160px;
        width: 160px;
        margin: 10px auto;
        padding-bottom: 5px;
        margin-bottom: 5px;
    }
    .card .card-img-wrapper img {
        height: 100%;
        width: 100%;
        border-radius: 50%;
    }
    .card .card-footer {
        margin-top: 20px;
    }
    .card .card-footer .footer-box {
        position: relative;
        border-top: 2px solid #ff9b9b;
        box-shadow: 0 3px 6px -1px rgb(0 0 0 / 26%), 0 2px 4px -1px rgb(0 0 0 / 6%);
        border-radius: 5px;
        margin: 0 auto;
        padding: 10px;
        display: flex;
        justify-content: space-around;
    }
    .card .card-footer .footer-box .box-wrapper {
        position: relative;
        padding: 10;
    }
    .card .card-footer .footer-box .box-wrapper .box-text {
        font-size: 12px;
        font-weight: 600;
        color: #00000085;
        letter-spacing: 0.5px;
    }
</style>


<section class="organisers">
    {% for organiser in site.data.organisers %}

    <div class="card">
        <div class="cover"></div>
        <div class="card-wrapper">
            <div class="card-header">
                <div class="card-img-wrapper">
                    <img src="{{ site.baseurl }}/assets/img/{{ organiser.img }}"/>
                </div>
                <h1 class="card-title">{{ organiser.name }}</h1>
                <p class="card-desc">{{ organiser.level }} Student at {{ organiser.school }}</p>
            </div>
            <div class="card-footer">
                <div class="footer-box">
                    {% for comm in organiser.comms %}
                    <div class="box-wrapper">
                        <div class="box-text">{{ comm }}</div>
                    </div>
                    {% endfor %}
                </div>
            </div>
        </div>
    </div>

    {% endfor %}
</section>

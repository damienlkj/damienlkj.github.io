---
layout: page
permalink: /education/undergraduate/
title: Undergraduate
full-width: True
---

<h1 style="text-align: center;">National University of Singapore, 2020 - 2023</h1>
<h2 style="text-align: center;"> Bachelor of Engineering (Chemical Engineering)</h2>
<h3 style="text-align: center;"> Minor in Computer Science</h3>
<h3 style="text-align: center;"> Minor in Engineering Materials</h3>  
<h4 style="text-align: center;"> GPA/CAP: 4.90/5.00 &emsp; &emsp; Total credits: 200</h4>  
&nbsp;
<p style="text-align: center;"><b>Courses taken</b></p>

{% tabs log %}
{% tab log Year 1 %}
{% include_relative undergraduate/year1.html %}
{% endtab %}

{% tab log Year 2 %}
{% include_relative undergraduate/year2.html %}
{% endtab %}

{% tab log Year 3 %}
{% include_relative undergraduate/year3.html %}
{% endtab %}
{% endtabs %}

<script src="/assets/js/tabs.js"></script>

<style>
    .tab {
    display: flex;
    flex-wrap: wrap;
    padding: 0;
    list-style: none;
    width: 500px;
    margin: 0 auto;
    justify-content: center;
}

.tab > * {
    flex: none;
    padding-left: 20px;
    position: relative;
}

.tab > * > a {
    display: block;
    text-align: center;
    padding: 9px 20px;
    color: #999;
    border-bottom: 2px solid transparent;
    border-bottom-color: transparent;
    text-transform: uppercase;
    transition: color .1s ease-in-out;
    line-height: 20px;
}

.tab > .active > a {
    color:#222;
    border-color: #1e87f0;
}

.tab > li > a {
    text-decoration: none;
    cursor: pointer;
}

.tab-content {
    padding: 0;
}

.tab-content > li {
    display: none;
}
.tab-content > li.active {
    display: initial;
}
</style>
---
layout: page
permalink: /education/masters/
title: Masters
full-width: True
---

<h1 style="text-align: center;">National University of Singapore, 2023 - 2024</h1>
<h2 style="text-align: center;"> Master of Science (Materials Science and Engineering)</h2>
<div class="container">
  <div class=item><b>GPA:</b> 5.00/5.00 </div>
  <div class=item><b>Grade Breakdown:</b> 9A+/1A </div>
  <div class=item><b>Total credits:</b> 40/40 </div>
</div>
<p style="text-align: center;"><b>Courses taken</b></p>

<div class="tab-container">
    <div class="bar">
        <button class="tablinks selected" onclick="openTab(event, 'sem_1')">Semester 1</button>
        <button class="tablinks" onclick="openTab(event, 'sem_2')">Semester 2</button>
    </div>
    <div id="sem_1" class="tabcontent active">
        {% for course in site.data.modules.Sem7 %}
            <details>
            <summary>
                <b>{{ course[0] }}: {{ course[1].title }}</b>
                <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
            </summary>
            <p>{{ course[1].description }}</p>
            </details>
        {% endfor %}
    </div>
    <div id="sem_2" class="tabcontent">
        {% for course in site.data.modules.Sem8 %}
            <details>
            <summary>
                <b>{{ course[0] }}: {{ course[1].title }}</b>
                <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
            </summary>
            <p>{{ course[1].description }}</p>
            </details>
        {% endfor %}
    </div>
</div>

<script>
  function openTab(evt, sem) {
    var i, tabcontent, tablinks;
    tabcontent = document.getElementsByClassName("tabcontent");
    for (i = 0; i < tabcontent.length; i++) {
        tabcontent[i].style.display = "none";
        tabcontent[i].className = tabcontent[i].className.replace(" active", "");
    }
    tablinks = document.getElementsByClassName("tablinks");
    for (i = 0; i < tablinks.length; i++) {
        tablinks[i].className = tablinks[i].className.replace(" selected", "");
    }
    document.getElementById(sem).style.display = "block";
    document.getElementById(sem).className += " active";
    evt.currentTarget.className += " selected";
    }
</script>

<style>
    .container {
    display: grid;
    text-align: center;
    padding-top: 20px;
    font-family: 'Open Sans';
    }

    @media screen and (min-width:700px) {
        .container {
        grid-template-columns: 33% 33% 33%
        }
    }

    .tab-container {
    border: None;
    padding: 0px;
    align-items: center;
    text-align: center;
    }

    button {
    background-color: #f1f1f1;
    border: none;
    padding: 10px 20px;
    cursor: pointer;
    transition: background-color 0.3s;
    }

    .tabcontent {
    display: none;
    text-align: left;
    border: 1px solid #ccc;
    padding: 20px;
    }

    .selected {
        background-color: #474747;
        color: #f1f1f1;
    }

    .active {
        display: block;
    }

    .bar {
    display: inline-block;
    margin-bottom: 10px;
    }
   
</style>
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
<div class="container">
  <div class=item><b>GPA:</b> 4.87/5.00 </div>
  <div class=item><b>Grade Breakdown:</b> 21A+/9A/8A- </div>
  <div class=item><b>Total credits:</b> 200/160 </div>
</div>

<p style="text-align: center;"><b>Courses taken</b></p>

<div class="tab-container"> 
  <div class="bar">
    <button class="parent_tab selected" onclick="openParentTab(event, 'Year 1')">Year 1</button>
    <button class="parent_tab" onclick="openParentTab(event, 'Year 2')">Year 2</button>
    <button class="parent_tab" onclick="openParentTab(event, 'Year 3')">Year 3</button>
  </div>

  <div id="Year 1" class="child-container">
    <div class="childbar">
      <button class="child_tab selected" onclick="openChildTab(event, 'sem1')">Semester 1</button>
      <button class="child_tab" onclick="openChildTab(event, 'sem2')">Semester 2</button>
      <button class="child_tab" onclick="openChildTab(event, 'st1')">Special Term / Others</button>
    </div>
    <div id="sem1" class="tabcontent">
        {% for course in site.data.modules.Sem1 %}
            <details>
            <summary>
                <b>{{ course[0] }}: {{ course[1].title }}</b>
                <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
            </summary>
            <p>{{ course[1].description }}</p>
            </details>
        {% endfor %}
    </div>
    <div id="sem2" class="tabcontent">
        {% for course in site.data.modules.Sem2 %}
            <details>
            <summary>
                <b>{{ course[0] }}: {{ course[1].title }}</b>
                <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
            </summary>
            <p>{{ course[1].description }}</p>
            </details>
        {% endfor %}
    </div>
    <div id="st1" class="tabcontent child">
        {% for course in site.data.modules.year1st %}
            <details>
            <summary>
                <b>{{ course[0] }}: {{ course[1].title }}</b>
                {% if course[0] == "EG1311" %}
                <p><i>Done as Advanced Placement Credits (APC)</i></p>
                {% endif %}
                <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
            </summary>
            <p>{{ course[1].description }}</p>
            </details>
        {% endfor %}
        <details>
            <summary>
            <b>PV1x: Solar Energy: Photovoltaic (PV) Energy Conversion</b>
            <p><i>Done as Design your Own Module (DYOM)</i></p>
            <p><b>Grade: CS</b> &emsp; Credits: 5 &emsp;<a href="https://courses.edx.org/certificates/8ec3c2b8e37a41aea3c3240abd798e1e">Certificate</a></p>
            </summary>
            <p>The key factor in getting more efficient and cheaper solar energy panels is the advance in the development of photovoltaic cells. In this course, you will learn how photovoltaic cells convert solar energy into usable electricity. You will also discover how to tackle potential loss mechanisms in solar cells. By understanding the semiconductor physics and optics involved, you will develop in-depth knowledge of how a photovoltaic cell works under different conditions. You will learn how to model all aspects of a working solar cell. For engineers and scientists working in the photovoltaic industry, this course is an absolute must to understand the opportunities for solar cell innovation.</p>
        </details>

        <details>
            <summary>
            <b>PV2x: Solar Energy: Photovoltaic (PV) Technologies</b>
            <p><i>Done as Design your Own Module (DYOM)</i></p>
            <p><b>Grade: CS</b> &emsp; Credits: 3 &emsp;<a href="https://courses.edx.org/certificates/49b58a1d11fd41a8a8e2b7e244658cc6">Certificate</a></p>
            </summary>
            <p>The technologies used to produce solar cells and photovoltaic modules are advancing to deliver highly efficient and flexible solar panels. In this course you will explore the main PV technologies in the current market. You will gain in-depth knowledge about crystalline silicon based solar cells (90% market share) as well as other up and coming technologies like CdTe, CIGS and Perovskites. This course provides answers to the questions: How are solar cells made from raw materials? Which technologies have the potential to be the major players for different applications in the future? What different techniques are used for the processing and characterization of the various PV technologies?</p>
        </details>
    </div>

  </div>

  <div id="Year 2" class="child-container">
    <div class="childbar">
      <button class="child_tab selected" onclick="openChildTab(event, 'sem3')">Semester 1</button>
      <button class="child_tab" onclick="openChildTab(event, 'sem4')">Semester 2</button>
      <button class="child_tab" onclick="openChildTab(event, 'st2')">Special Term / Others</button>
    </div>
    <div id="sem3" class="tabcontent">
        {% for course in site.data.modules.Sem3 %}
            <details>
            <summary>
                <b>{{ course[0] }}: {{ course[1].title }}</b>
                <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
            </summary>
            <p>{{ course[1].description }}</p>
            </details>
        {% endfor %}
    </div>
    <div id="sem4" class="tabcontent">
        {% for course in site.data.modules.Sem4 %}
            <details>
            <summary>
                <b>{{ course[0] }}: {{ course[1].title }}</b>
                {% if course[0] == "EG2605" %}
                <p><i>Research under Assistant Professor He Qian's group</i></p>
                {% endif %}
                <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
            </summary>
            <p>{{ course[1].description }}</p>
            </details>
        {% endfor %}
    </div>
    <div id="st2" class="tabcontent">
        {% for course in site.data.modules.year2st %}
            <details>
            <summary>
                <b>{{ course[0] }}: {{ course[1].title }}</b>
                {% if course[0] == "EG2701A" %}
                <p><i>Research under Assistant Professor Pieremanuele Canepa's group</i></p>
                {% endif %}
                <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
            </summary>
            <p>{{ course[1].description }}</p>
            </details>
        {% endfor %}
        <details>
            <summary>
            <b>IWC207: Statistics</b>
            <p><i>Done in Korea University (Winter School)</i></p>
            <p><b>Grade: A+</b> &emsp; Credits: 4 </p>
            </summary>
            <p>This course provides a broad introduction to statistical practice and data analysis techniques. It aims to equip students with a basic understanding of statistics, so that they can employ appropriate methods of analysis in various circumstances. The techniques learnt are widely used in the sciences, social sciences, business and many other fields of study. Topics covered include collecting data, getting information from data, data manipulation, statistical inference, regression and analysis of categorical data.</p>
        </details>
    </div>

  </div>

  <div id="Year 3" class="child-container">
    <div class="childbar">
      <button class="child_tab selected" onclick="openChildTab(event, 'sem5')">Semester 1</button>
      <button class="child_tab" onclick="openChildTab(event, 'sem6')">Semester 2</button>
    </div>
    <div id="sem5" class="tabcontent">
    {% for course in site.data.modules.Sem5 %}
        <details>
        <summary>
            <b>{{ course[0] }}: {{ course[1].title }}</b>
            {% if course[0] == "EG3611A" %}
            <p><i>Research intern in the Agency for Science, Technology and Research (A*STAR)</i></p>
            {% endif %}
            <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
        </summary>
        <p>{{ course[1].description }}</p>
        </details>
    {% endfor %}
    </div>
    <div id="sem6" class="tabcontent">
    {% for course in site.data.modules.Sem6 %}
        <details>
        <summary>
            <b>{{ course[0] }}: {{ course[1].title }}</b>
            {% if course[0] == "CN4118" %}
            <p><i>Research under Professor Karimi's group</i></p>
            {% endif %}
            <p><b>Grade: {{ course[1].grade }}</b> &emsp; Credits: {{ course[1].credit }}</p>
        </summary>
        <p>{{ course[1].description }}</p>
        </details>
    {% endfor %}
    </div>
  </div>
</div>

<script>
  function openParentTab(evt, year) {
    var i, x, tablinks;
    x = document.getElementsByClassName("child-container");
    for (i = 0; i < x.length; i++) {
      x[i].style.display = "none";
    }
    x = document.getElementsByClassName("parent_tab");
    for (i = 0; i < x.length; i++) {
      x[i].className = x[i].className.replace(" selected", "");
    }
    to_show = document.getElementById(year)
    to_show.style.display = "block"
    evt.currentTarget.className += " selected";
  }

  function openChildTab(evt, sem) {
    var i, x, tablinks;
    x = document.getElementsByClassName("tabcontent");
    for (i = 0; i < x.length; i++) {
      x[i].style.display = "none";
    }
    x = document.getElementsByClassName("child_tab");
    for (i = 0; i < x.length; i++) {
      x[i].className = x[i].className.replace(" selected", "");
    }
    to_show = document.getElementById(sem)
    to_show.style.display = "block"
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

.tabcontent {
  text-align: left;
  border: 1px solid #ccc;
  padding: 20px;
}

.bar {
  align-items: center;
}

button {
  background-color: #f1f1f1;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.selected {
  background-color: #474747;
  color: #f1f1f1;
}

.bar {
  display: inline-block;
  margin-bottom: 10px;
}

</style>
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

<div class="tab-container"> 
  <div class="bar">
    <button class="item button tablink selected" onclick="openTab(event, 'year', 'Year 1', 'tablink')">Year 1</button>
    <button class="item button tablink" onclick="openTab(event, 'year', 'Year 2', 'tablink')">Year 2</button>
    <button class="item button tablink" onclick="openTab(event, 'year', 'Year 3', 'tablink')">Year 3</button>
  </div>

  <div id="Year 1" class="tab-container  year">
    <div class="bar">
      <button class="item button tablink2 selected" onclick="openTab(event, 'child', 'sem1', 'tablink2')">Semester 1</button>
      <button class="item button tablink2" onclick="openTab(event, 'child', 'sem2', 'tablink2')">Semester 2</button>
      <button class="item button tablink2" onclick="openTab(event, 'child', 'st1', 'tablink2')">Special Term / Others</button>
    </div>
    <div id="sem1" class="tab-container  child">
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
    <div id="sem2" class="tab-container  child" style="display:none">
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
    <div id="st1" class="tab-container  child" style="display:none">
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

  <div id="Year 2" class="tab-container  year" style="display:none">
    <div class="bar">
      <button class="item button tablink2 selected" onclick="openTab(event, 'child', 'sem3', 'tablink2')">Semester 1</button>
      <button class="item button tablink2" onclick="openTab(event, 'child', 'sem4', 'tablink2')">Semester 2</button>
      <button class="item button tablink2" onclick="openTab(event, 'child', 'st2', 'tablink2')">Special Term / Others</button>
    </div>
    <div id="sem3" class="tab-container  child" style="display:none">
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
    <div id="sem4" class="tab-container  child" style="display:none">
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
    <div id="st2" class="tab-container  child" style="display:none">
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
            <p><b>Grade: CS</b> &emsp; Credits: 4 </p>
            </summary>
            <p>This course provides a broad introduction to statistical practice and data analysis techniques. It aims to equip students with a basic understanding of statistics, so that they can employ appropriate methods of analysis in various circumstances. The techniques learnt are widely used in the sciences, social sciences, business and many other fields of study. Topics covered include collecting data, getting information from data, data manipulation, statistical inference, regression and analysis of categorical data.</p>
        </details>
    </div>

  </div>

  <div id="Year 3" class="tab-container  year" style="display:none">
    <div class="bar">
      <button class="item button tablink2 selected" onclick="openTab(event, 'child', 'sem5', 'tablink2')">Semester 1</button>
      <button class="item button tablink2" onclick="openTab(event, 'child', 'sem6', 'tablink2')">Semester 2</button>
    </div>
    <div id="sem5" class="tab-container  child" style="display:none">
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
    <div id="sem6" class="tab-container  child" style="display:none">
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
  function openTab(evt, tabBarName, cityName, tablinkName) {
    var i, x, tablinks;
    x = document.getElementsByClassName(tabBarName);
    for (i = 0; i < x.length; i++) {
      x[i].style.display = "none";
    }
    tablinks = document.getElementsByClassName(tablinkName);
    for (i = 0; i < x.length; i++) {
      tablinks[i].className = tablinks[i].className.replace(" selected", "");
    }
    document.getElementById(cityName).style.display = "block";
    evt.currentTarget.className += " selected";
  }
</script>

<style>
.tab-container {
  border: None;
  padding: 0px;
  align-items: center;
  text-align: center;
}

.selected {
  background-color: #fff;
}

.item {
  background-color: #f1f1f1;
  border: none;
  padding: 10px 20px;
  cursor: pointer;
  transition: background-color 0.3s;
}

.bar {
    display: inline-block;
    margin-bottom: 10px;
}

.child {
    text-align: left;
    border: 1px solid #ccc;
    padding: 20px
}
</style> 
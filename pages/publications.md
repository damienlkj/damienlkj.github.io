---
layout: page
title: Publications
permalink: /publications/
full-width: true
---

{% assign sorted_papers = site.papers | sort:"number" | reverse %}

<ol type="1">
  {% assign counter = sorted_papers.size %}
  {% assign year = 2025 %}

  {% for page in sorted_papers %}
    {% if page.year != year %}
      <h1>{{ year | minus:1 }}</h1>
      {% assign year = page.year %}
    {% endif %}
    <a href="{{ page.url }}">
      <li class="list-item">
        <img src="{{ page.image }}" alt="Image">
        {{ counter }}. {{ page.title }}
      </li>
    </a>
    {% assign counter = counter | minus: 1 %}
  {% endfor %}
</ol>

<style>
  .list-item {
    display: flex;
    align-items: center;
    padding: 5px;
  }
  
  .list-item img {
    width: 150px; /* Adjust the width as per your requirement */
    height: auto; /* Maintain aspect ratio */
    margin-right: 20px; /* Add spacing between image and text */
  }

  a {
    color: black; /* Set the desired color for the hyperlink */
    text-decoration: none; /* Remove the underline */
  }
  
</style>

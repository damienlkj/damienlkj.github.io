---
layout: page
title: Education
permalink: /education/
---

<div class="responsive">
    <div class="gallery">
        <a href="/education/undergraduate" class="square-button">
            <img src="/assets/img/nus-logo-svg-vector.svg" alt="Undergraduate" width="300" height="300">
            <span class="button-text">Undergraduate</span>
        </a>
        <a href="/education/masters" class="square-button">
            <img src="/assets/img/nus-logo-svg-vector.svg" alt="Master" width="300" height="300">
            <span class="button-text">Masters</span>
        </a>
        <a href="/education/phd" class="square-button">
            <img src="/assets/img/epfl.png" alt="PhD" width="300">
            <span class="button-text">PhD</span>
        </a>
    </div>
</div>

<style>
.square-button {
  display: flex;
  flex-direction: column;
  justify-content: flex-end;
  align-items: center;
  text-decoration: none;
  background-color: #e0e0e0;
  border-radius: 8px;
  width: 300px; /* Adjust the width as needed */
  height: 300px; /* Adjust the height as needed */
  transition: background-color 0.3s;
  position: relative;
}

.square-button:hover {
  background-color: #c0c0c0;
}

.square-button img {
  max-width: 80%;
  max-height: 80%;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}

.square-button .button-text {
  margin-top: auto;
  font-weight: bold;
  color: #333;
  padding-bottom: 16px;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  grid-gap: 10px;
}

.responsive {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  align-items: center;
}

@media (max-width: 767px) {
  .gallery {
    grid-template-columns: 1fr; /* Change to one column on smaller screens */
  }

  .square-button {
    width: 100%; /* Set button width to full width on smaller screens */
    margin-bottom: 10px; /* Add some vertical spacing between buttons */
  }
}
</style>

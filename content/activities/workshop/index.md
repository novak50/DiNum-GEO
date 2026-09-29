---
title: First Project Activity – Workshop
date: 2026-08-24

# Also list this activity on the News page.
show_in_news: true

authors:
  - me
  - ksenija
  - milos

categories:
  - Research

tags:
  - Academic
  - Research

image:
  preview_only: true
  caption:

summary:

---

The first activity of the project, a one-day workshop titled "From Open Geodata and Ground Models to Advanced BIM-FEM Analysis," was held on 24 August 2026 at the Faculty of Civil Engineering, University of Belgrade. The Serbian part of the DiNum team had the great honour of hosting our diaspora partners, Prof. Dr Jelena Ninić from Durham University and Dr Tijana Jovanović from the British Geological Survey.

In the introductory part of the workshop, project coordinator Dr Miloš Marjanović had the opportunity to introduce the audience to the project, the call within the Science Fund, as well as past and upcoming activities. Afterwards, team members Ksenija Micić and Novak Joksimović presented the project's results to date and outlined future improvements.

The central part of the event consisted of highly interesting hands-on lectures by our partners: Dr Ninić on "Advanced computational modelling for underground infrastructure" and Dr Jovanović on "Hidden potential of open data."

The workshop brought together interested students, colleagues from other faculties, as well as colleagues from industry, and judging by the number of questions and ideas, as well as the quality of the open discussions, it can safely be said that it was a great success!

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "workshop_1.jpg" >}}" alt="Workshop participants in the lecture hall" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="{{< bundle-url "workshop_2.jpg" >}}" alt="Dr Tijana Jovanović presenting" style="width: 100%; height: 400px; object-fit: contain; background: #f3f4f6; border-radius: 8px; display: none;">
    <img src="{{< bundle-url "workshop_3.jpg" >}}" alt="Prof. Dr Jelena Ninić presenting" style="width: 100%; height: 400px; object-fit: contain; background: #f3f4f6; border-radius: 8px; display: none;">
    <img src="{{< bundle-url "workshop_4.jpg" >}}" alt="The DiNum-GEO team at the workshop" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: none;">
  </div>

  <button onclick="dinumgeoCarouselMove(-1)"
    style="position: absolute; left: 8px; top: 50%; transform: translateY(-50%); background: rgba(0,0,0,0.4); color: white; border: none; width: 40px; height: 40px; border-radius: 50%; cursor: pointer; font-size: 20px;">
    ‹
  </button>

  <button onclick="dinumgeoCarouselMove(1)"
    style="position: absolute; right: 8px; top: 50%; transform: translateY(-50%); background: rgba(0,0,0,0.4); color: white; border: none; width: 40px; height: 40px; border-radius: 50%; cursor: pointer; font-size: 20px;">
    ›
  </button>
</div>

<script>
  let dinumgeoCarouselIndex = 0;
  function dinumgeoCarouselMove(direction) {
    const images = document.querySelectorAll('#carousel-images img');
    images[dinumgeoCarouselIndex].style.display = 'none';
    dinumgeoCarouselIndex = (dinumgeoCarouselIndex + direction + images.length) % images.length;
    images[dinumgeoCarouselIndex].style.display = 'block';
  }
</script>

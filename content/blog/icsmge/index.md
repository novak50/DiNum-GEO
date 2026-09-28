---
title: ICSMGE Conference
date: 2026-06-14

authors:
  - me

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

At the world conference "21st International Conference on Soil Mechanics and Geotechnical Engineering," held from 14 to 19 June 2026 in Vienna, Austria, the DiNum team presented its results through the paper "GIM-to-FEM: From Digital Ground Information Models to Probabilistic Numerical Analysis of Underground Structures," in collaboration with the University of Birmingham. Beyond the great company, meeting new colleagues and collaborators, and enjoying the lectures and the city, the DiNum team representatives also had the opportunity to exchange numerous experiences on complementary modelling topics, as well as to receive valuable suggestions and advice for further advancing the research and its application in practice.

More about the event at the link: [ICSMGE 2026](https://www.icsmge2026.org/en/).
More about the publication at the link: ***.

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="icsmge_1.jpg" alt="Presentation of the GIM-to-FEM paper at ICSMGE 2026" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="icsmge_2.jpg" alt="DiNum-GEO team members at ICSMGE 2026 in Vienna" style="width: 100%; height: 400px; object-fit: contain; background: #f3f4f6; border-radius: 8px; display: none;">
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

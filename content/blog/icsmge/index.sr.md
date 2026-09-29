---
title: "ICSMGE konferencija"
date: 2026-06-14

authors:
  - me

categories:
  - Istraživanje

tags:
  - Akademsko
  - Istraživanje

image:
  preview_only: true
  caption:

summary:
---

Na svetskoj konferenciji „21st International Conference on Soil Mechanics and Geotechnical Engineering”, održanoj od 14. do 19. juna 2026. godine u Beču, u Austriji, tim DiNum predstavio je svoje rezultate kroz rad „GIM-to-FEM: From Digital Ground Information Models to Probabilistic Numerical Analysis of Underground Structures”, nastao u saradnji sa Univerzitetom u Birmingemu. Pored sjajnog društva, upoznavanja novih kolega i saradnika i uživanja u predavanjima i gradu, predstavnici tima DiNum imali su priliku i da razmene brojna iskustva o komplementarnim temama modeliranja, kao i da dobiju dragocene sugestije i savete za dalje unapređenje istraživanja i njegove primene u praksi.

Više o događaju na linku: [ICSMGE 2026](https://www.icsmge2026.org/en/).
Više o publikaciji na linku: ***.

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "icsmge_1.jpg" >}}" alt="Predstavljanje rada GIM-to-FEM na konferenciji ICSMGE 2026" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="{{< bundle-url "icsmge_2.jpg" >}}" alt="Članovi tima DiNum-GEO na konferenciji ICSMGE 2026 u Beču" style="width: 100%; height: 400px; object-fit: contain; background: #f3f4f6; border-radius: 8px; display: none;">
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

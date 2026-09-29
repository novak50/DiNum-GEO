---
title: "SETC"
date: 2025-10-03

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

cover:
  image: SETC_1.jpg
  style: "gradient"
  height: "large"
  position:
    x: 50
    y: 50

  fade:
    enabled: true
---

Prva publikacija pod nazivom „Computer-aided ground modelling including soil spatial variability for geotechnical applications”, rezultat posvećenog i napornog rada na projektu, predstavljena je na konferenciji „Southeastern Europe Tunnelling Conference”, održanoj od 1. do 3. oktobra 2025. godine u Sava centru u Beogradu. Ovaj događaj bio je odlična prilika da se originalni rezultati naučnog istraživanja predstave domaćoj i stranoj publici iz vodećih svetskih naučnih institucija, kao i brojnim kolegama iz privrede. Pored konstruktivnih diskusija, komentara i razmene ideja, tim DiNum iz Srbije iskoristio je ovu konferenciju da postavi temelje za pokretanje značajnih naučnih saradnji sa kolegama iz privrede.
Više o publikaciji na linku: ***.

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "SETC_1.jpg" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="{{< bundle-url "SETC_2.jpeg" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
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
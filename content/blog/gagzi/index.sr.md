---
title: "GAGZI konferencija"
date: 2025-10-17

authors:
  - me
  - ksenija
  - milos

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
  image: GAGZI_2.jpeg
  style: "gradient"
  height: "large"
  position:
    x: 50
    y: 50

  fade:
    enabled: true
---

Na međunarodnoj naučno-stručnoj konferenciji „Geotehnički aspekti građevinarstva i zemljotresno inženjerstvo”, održanoj od 15. do 17. oktobra 2025. godine, tim DiNum predstavio je naučne rezultate projekta kroz rad „BIM-enabled digital modelling and simulation of block-in-matrix material”. Rad je privukao značajnu pažnju publike, uz brojne diskusije i komentare koji će biti iskorišćeni za unapređenje metodologije i alata. Ova konferencija bila je još jedna odlična prilika za umrežavanje sa kolegama iz akademske zajednice i privrede iz Srbije i regiona.
Više o publikaciji na linku: ***.

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "GAGZI_1.jpeg" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="{{< bundle-url "GAGZI_2.jpeg" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: none;">
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
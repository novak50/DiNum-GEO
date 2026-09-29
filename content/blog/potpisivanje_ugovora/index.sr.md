---
title: "Potpisivanje ugovora"
date: 2025-06-10

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
  image: potpisivanje_ugovora_2.JPG
  style: "gradient"
  height: "large"
  position:
    x: 50
    y: 0

  fade:
    enabled: true
---

Aktivnosti na projektu u okviru Programa saradnje srpske nauke sa dijasporom – Podrška istraživačkim posetama naučnika iz dijaspore započele su potpisivanjem ugovora u prostorijama Fonda za nauku Republike Srbije 10.06.2025. godine. Potpisivanju ugovora, u ime tima DiNum-GEO, prisustvovao je rukovodilac projekta doc. dr Miloš Marjanović sa Građevinskog fakulteta Univerziteta u Beogradu. Ovo je bila odlična prilika za upoznavanje sa istraživačima iz drugih naučnoistraživačkih organizacija, razmenu ideja i konstruktivne razgovore o unapređenju i razvoju naučnog sistema u Republici Srbiji. Više o događaju na linku: [Potpisivanje ugovora](https://fondzanauku.gov.rs/2025/07/kick-off-sastanak-povodom-pocetka-realizacije-projekata-u-okviru-programa-dijaspora-istrazivacke-posete/).

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "potpisivanje_ugovora_1.JPG" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="{{< bundle-url "potpisivanje_ugovora_2.JPG" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
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
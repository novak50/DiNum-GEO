---
title: Signing of contract
date: 2025-06-10

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

Project activities under the Program of Cooperation between Serbian Science and the Diaspora – Support for Research Visits of Diaspora Scientists began with the signing of the contract at the premises of the Science Fund of the Republic of Serbia on 10.06.2025. The contract signing was attended, on behalf of the DiNum-GEO team, by the project coordinator Assist. Prof. Dr. Miloš Marjanović from the Faculty of Civil Engineering, University of Belgrade. This was a great opportunity to meet researchers from other scientific research institutions, exchange ideas, and hold constructive discussions on improving and developing the scientific system in the Republic of Serbia. More about the event at the link: [Contract signing](https://fondzanauku.gov.rs/2025/07/kick-off-sastanak-povodom-pocetka-realizacije-projekata-u-okviru-programa-dijaspora-istrazivacke-posete/).

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="potpisivanje_ugovora_1.JPG" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="potpisivanje_ugovora_2.JPG" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
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
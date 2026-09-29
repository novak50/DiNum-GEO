---
title: "Kongres geologa Srbije"
date: 2026-06-03

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

U skladu sa misijom projekta da promoviše neraskidivu vezu između geološkog i geotehničkog inženjerstva, DiNum-GEO je predstavljen i na 19. Kongresu geologa Srbije, održanom od 3. do 6. juna na Borskom jezeru. Bilo nam je i zadovoljstvo i izazov da kolegama geolozima u sažetom obliku približimo naš projekat i njegov značaj. Sudeći po njihovim reakcijama, pitanjima i diskusijama, čini se da smo u tome uspeli! U istraživačkom radu od velikog je značaja čuti mišljenja stručnjaka iz komplementarnih oblasti, uvažiti ih i na odgovarajući način primeniti. Ideje i sugestije koje smo doneli sa Kongresa sigurno će naći svoje mesto u narednim fazama našeg istraživanja.

Više o događaju na linku: [Kongres geologa Srbije](https://19kongres.sgd.rs/).
Više o publikaciji na linku: [Ka integrisanom digitalnom i numeričkom modeliranju za optimizaciju u geotehničkom inženjerstvu]({{< relref "/papers/kgs-2026-integrated-digital-numerical-modelling/index.md" >}}).

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "kgs_1.jpg" >}}" alt="Predstavljanje projekta DiNum-GEO na 19. Kongresu geologa Srbije" style="width: 100%; height: 400px; object-fit: contain; background: #f3f4f6; border-radius: 8px; display: block;">
    <img src="{{< bundle-url "kgs_2.jpg" >}}" alt="Naslovni slajd: Ka integrisanom digitalnom i numeričkom modeliranju za optimizaciju u geotehničkom inženjerstvu" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: none;">
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

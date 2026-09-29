---
title: "Kick-off sastanak"
date: 2025-10-17

# Also list this activity on the News page.
show_in_news: true

authors:
  - me
  - ksenija
  - milos
  - "Tijana Jovanović"
  - "Jelena Ninić"

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

Uvodni (kick-off) sastanak projekta DiNum-GEO održan je 16.10.2025. godine u onlajn formatu. Sastanku su prisustvovali svi članovi našeg multidisciplinarnog tima. Ovo onlajn povezivanje okupilo je predstavnike vodećih svetskih institucija u oblastima geotehnike, digitalnog inženjerstva i upravljanja geoprostornim podacima – Građevinskog fakulteta Univerziteta u Beogradu, Univerziteta u Daramu i Britanskog geološkog zavoda. Tim iz Srbije je, zajedno sa partnerima iz dijaspore dr Jelenom Ninić i dr Tijanom Jovanović, utvrdio opšti plan aktivnosti na projektu i dogovorio detalje u vezi sa realizacijom istraživačkih poseta.

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "kickoff_zoom.png" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
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
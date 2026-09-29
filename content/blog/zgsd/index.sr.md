---
title: "Predstavljanje rada na Zboru SGD"
date: 2025-12-24

authors:
  - ksenija

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
  image: ZSGD.jpeg
  style: "gradient"
  height: "large"
  position:
    x: 50
    y: 100


  fade:
    enabled: true
---

S obzirom na to da inženjerskogeološko modeliranje terena ima veoma važnu ulogu u konceptu i metodologiji projekta DiNum-GEO, rezultati projekta predstavljeni su i geološkoj publici na Zboru Srpskog geološkog društva, održanom 24.12.2025. godine u prostorijama Rudarsko-geološkog fakulteta. Tom prilikom članica tima i doktorantkinja na Katedri za geotehniku ovog fakulteta, Ksenija Micić, predstavila je rad „3D litološko modeliranje u GIS okruženju: uticaj obima i prostornog rasporeda istražnih bušotina”, objavljen u časopisu nacionalnog značaja „Zapisnici Srpskog geološkog društva”. Pored uspostavljanja naučne saradnje sa partnerima iz dijaspore, za tim DiNum je od velikog značaja i jačanje saradnje sa kolegama i stručnjacima sa Univerziteta u Beogradu, čemu je učešće na ovom događaju značajno doprinelo.
Više o događaju na linku: https://sgd.rs/odrzan-redovni-zbor-srpskog-geolosko/.
Više o publikaciji na linku: [3D litološko modeliranje u GIS okruženju]({{< relref "/papers/zsgd-2026-voxel-lithological-modelling/index.md" >}}).

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "ZSGD.jpeg" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
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
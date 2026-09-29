---
title: "ACUUS konferencija"

date: 2025-11-07

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

summary: "Na svetskoj konferenciji „19th World Conference of the Associated Research Centres for the Urban Underground Space”, održanoj od 4. do 7. novembra 2025. u Sava centru u Beogradu, tim DiNum predstavio je rad „Towards an Advanced Geotechnical Modelling of Block-in-Matrix Rock for Robust Tunnel Design and Construction”"

cover:
  image: ACUUS_2.jpeg
  style: "gradient"
  height: "large"
  position:
    x: 50
    y: 0

  fade:
    enabled: true
---

Na svetskoj konferenciji „19th World Conference of the Associated Research Centres for the Urban Underground Space”, održanoj od 4. do 7. novembra 2025. godine u Sava centru u Beogradu, tim DiNum je, u saradnji sa Univerzitetom u Ljubljani, predstavio rad „Towards an Advanced Geotechnical Modelling of Block-in-Matrix Rock for Robust Tunnel Design and Construction”. Značaj i aktuelnost ideje koju DiNum-GEO promoviše, razvija i unapređuje ogleda se i u samoj temi konferencije – „Podzemna mobilnost i uzvišeno razmišljanje: nove mogućnosti i izazovi u korišćenju urbanog prostora” – kao i u svim naučnim doprinosima predstavljenim tokom četiri izuzetno produktivna i inspirativna dana u Sava centru. Tokom ove konferencije tim DiNum imao je jedinstvenu priliku da upozna svetske stručnjake u oblasti izgradnje tunela i prostornog planiranja i sa njima razmeni ideje i iskustva.
Više o publikaciji na linku: ***.

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "ACUUS_1.jpeg" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="{{< bundle-url "ACUUS_2.jpeg" >}}" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: none;">
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
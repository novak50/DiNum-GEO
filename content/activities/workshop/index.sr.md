---
title: "Prva projektna aktivnost – radionica"
date: 2026-08-24

# Also list this activity on the News page.
show_in_news: true

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
---

Prva aktivnost projekta, jednodnevna radionica pod nazivom „Od otvorenih geopodataka i modela terena do napredne BIM-MKE analize”, održana je 24. avgusta 2026. godine na Građevinskom fakultetu Univerziteta u Beogradu. Srpski deo tima DiNum imao je veliku čast da ugosti naše partnere iz dijaspore, prof. dr Jelenu Ninić sa Univerziteta u Daramu i dr Tijanu Jovanović iz Britanskog geološkog zavoda.

U uvodnom delu radionice rukovodilac projekta dr Miloš Marjanović imao je priliku da publici predstavi projekat, poziv Fonda za nauku, kao i dosadašnje i predstojeće aktivnosti. Nakon toga, članovi tima Ksenija Micić i Novak Joksimović predstavili su dosadašnje rezultate projekta i najavili buduća unapređenja.

Centralni deo događaja činila su izuzetno zanimljiva praktična predavanja naših partnera: dr Ninić na temu „Napredno računarsko modeliranje podzemne infrastrukture” i dr Jovanović na temu „Skriveni potencijal otvorenih podataka”.

Radionica je okupila zainteresovane studente, kolege sa drugih fakulteta, kao i kolege iz privrede, a sudeći po broju pitanja i ideja, kao i po kvalitetu otvorenih diskusija, slobodno se može reći da je bila veliki uspeh!

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="{{< bundle-url "workshop_1.jpg" >}}" alt="Učesnici radionice u amfiteatru" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="{{< bundle-url "workshop_2.jpg" >}}" alt="Predavanje dr Tijane Jovanović" style="width: 100%; height: 400px; object-fit: contain; background: #f3f4f6; border-radius: 8px; display: none;">
    <img src="{{< bundle-url "workshop_3.jpg" >}}" alt="Predavanje prof. dr Jelene Ninić" style="width: 100%; height: 400px; object-fit: contain; background: #f3f4f6; border-radius: 8px; display: none;">
    <img src="{{< bundle-url "workshop_4.jpg" >}}" alt="Tim DiNum-GEO na radionici" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: none;">
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

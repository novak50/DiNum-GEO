---
title: ACUUS Conference

date: 2025-11-07

authors:
  - me
  - ksenija
  - milos

categories:
  - Research

tags:
  - Academic
  - Research

image:
  preview_only: true
  caption:

summary: At the world conference “19th World Conference of the Associated Research Centres for the Urban Underground Space,” held from 4 to 7 November 2025 at the Sava Center in Belgrade, the DiNum team presented the paper 'Towards an Advanced Geotechnical Modelling of Block-in-Matrix Rock for Robust Tunnel Design and Construction'

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

At the world conference “19th World Conference of the Associated Research Centres for the Urban Underground Space,” held from 4 to 7 November 2025 at the Sava Center in Belgrade, the DiNum team presented the paper “Towards an Advanced Geotechnical Modelling of Block-in-Matrix Rock for Robust Tunnel Design and Construction,” in collaboration with the University of Ljubljana. The importance and relevance of the idea that DiNum-GEO promotes, develops, and advances is also reflected in the theme of the conference itself – “Underground mobility and elevated thinking: new opportunities and challenges in the use of urban space” – as well as in all the scientific contributions presented during four extremely productive and inspiring days at the Sava Center. During this conference, the DiNum team had a unique opportunity to meet and exchange ideas and experiences with world experts in the fields of tunnel construction and spatial planning. 
More about the publication at the link: ***************************************************. 

<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="ACUUS_1.jpeg" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
    <img src="ACUUS_2.jpeg" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: none;">
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
---
title: SGD Award
date: 2026-03-06

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
  image: nagrada.jpeg
  style: "gradient"
  height: "large"
  position:
    x: 50
    y: 50

  fade:
    enabled: true
---

On 06.03.2026, at the regular Assembly of the Serbian Geological Society, DiNum team member Ksenija Micić received the first prize of the Serbian Geological Society for the best scientific paper by young geologists and students for 2025 , for the paper “3D Voxel Lithological Modelling in a GIS Environment: The Influence of the Extent and Spatial Distribution of Exploratory Boreholes.” This recognition is further proof that the DiNum team is on the right scientific path, and serves as an incentive for all young colleagues to value their effort and work, to invest in their own progress and the progress of their research teams, and to continuously strengthen and improve the scientific system in the Republic of Serbia. 
More about the event at the link: [SGD](
https://sgd.rs/%d0%b3%d0%be%d0%b4%d0%b8%d1%88%d1%9a%d0%b8-%d0%ba%d0%be%d0%bd%d0%ba%d1%83%d1%80%d1%81-%d0%b7%d0%b0-%d0%bd%d0%b0%d1%98%d0%b1%d0%be%d1%99%d0%b8-%d1%80%d0%b0%d0%b4-%d0%bc%d0%bb%d0%b0%d0%b4%d0%b8%d1%85/).


<div style="position: relative; max-width: 700px; margin: 0 auto;">
  <div id="carousel-images">
    <img src="nagrada.jpeg" style="width: 100%; height: 400px; object-fit: cover; border-radius: 8px; display: block;">
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
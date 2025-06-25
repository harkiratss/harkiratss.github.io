---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a theoretical physicist currently working as a Research Associate at the Indian Institute of Technology Delhi. My research lies at the intersection of quantum theory and gravitation, exploring fundamental questions that arise when these two pillars of modern physics meet.

Here’s a glimpse into some of my recent research highlights.

<!-- Slideshow CSS -->
<style>
.slideshow-container {
  position: relative;
  max-width: 100%;
  margin: 2rem auto;
  text-align: center;
}

.slide {
  display: none;
}

.slide img {
  width: 48%;
  margin: 1%;
  vertical-align: top;
  border-radius: 6px;
}

.caption {
  font-style: italic;
  margin-top: 0.5rem;
  font-size: 0.95rem;
  max-width: 90%;
  margin-left: auto;
  margin-right: auto;
}

.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 45%;
  padding: 10px;
  color: black;
  font-weight: bold;
  font-size: 18px;
  background: #eee;
  border-radius: 4px;
  user-select: none;
  transition: background 0.3s;
}
.prev:hover, .next:hover {
  background: #ccc;
}
.prev {
  left: 0;
}
.next {
  right: 0;
}

.dots {
  text-align: center;
  margin-top: 1rem;
}
.dot {
  cursor: pointer;
  height: 12px;
  width: 12px;
  margin: 0 4px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.3s;
}
.dot.active {
  background-color: #333;
}
</style>

<div class="slideshow-container" id="slideshow">

  <div class="slide" style="display: flex;">
    <img src="/images/QC1.png" alt="QC1" />
    <img src="/images/QC2.png" alt="QC2" />
    <div class="caption">
      The quantum dynamics of the FLRW universe with dust and a positive cosmological constant depicting quantum. Heatmap shows the probability distribution associated with the wave packet; solid black curve = expectation value of volume, dotted = classical trajectory, dashed = uncertainty region. Top: broader Λ-distribution, Bottom: sharper Λ-distribution.
    </div>
  </div>

  <div class="slide">
    <img src="/images/QC3.png" alt="QC3" />
    <img src="/images/QC4.png" alt="QC4" />
    <div class="caption">
      The quantum dynamics of the FLRW universe with dust and a negative cosmological constant showing cyclic evolution. Heatmap shows the probability distribution associated with the wave packet; solid black curve = expectation value of volume, dotted = classical trajectory, dashed = uncertainty region. Top: coherent wave packet, Bottom: Gaussian wave packet with same mean Λ but sharper width.
    </div>
  </div>

  <div class="slide">
    <img src="/images/contour_plot_A=5.0.png" alt="Field Correlation" />
    <img src="/images/contour_plot_A=5.0_m.png" alt="Momentum Correlation" />
    <div class="caption">
      Quantum correlations of a test field propagating in a spacetime undergoing critical collapse, evaluated at the end of the numerical simulation. Dashed black lines = areal radius of apparent horizon, red dashed lines = location of apparent horizon. Top: field correlation, Bottom: momentum correlation.

  </div>

  <a class="prev" onclick="plusSlides(-1)">❮ Prev</a>
  <a class="next" onclick="plusSlides(1)">Next ❯</a>

  <div class="dots">
    <span class="dot" onclick="currentSlide(0)"></span>
    <span class="dot" onclick="currentSlide(1)"></span>
    <span class="dot" onclick="currentSlide(2)"></span>
  </div>
</div>

<script>
let slideIndex = 0;
let slides = document.querySelectorAll(".slide");
let dots = document.querySelectorAll(".dot");
let slideshow = document.getElementById("slideshow");
let timer = null;

function showSlide(n) {
  slides.forEach((slide, i) => {
    slide.style.display = i === n ? "flex" : "none";
    dots[i].classList.toggle("active", i === n);
  });
  slideIndex = n;
}

function plusSlides(n) {
  slideIndex = (slideIndex + n + slides.length) % slides.length;
  showSlide(slideIndex);
}

function currentSlide(n) {
  showSlide(n);
}

function autoSlide() {
  plusSlides(1);
}

function startAutoSlide() {
  timer = setInterval(autoSlide, 6000);
}

function pauseAutoSlide() {
  clearInterval(timer);
}

slideshow.addEventListener("mouseenter", pauseAutoSlide);
slideshow.addEventListener("mouseleave", startAutoSlide);

// Init
showSlide(slideIndex);
startAutoSlide();
</script>

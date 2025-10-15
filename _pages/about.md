---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a theoretical physicist currently working as an Institute Postdoctoral Fellow in the group of Prof. Dawood Kothawala at the Indian Institute of Technology Madras. Previously, I was as a Research Associate in the group of Prof. Suprit Singh at the Indian Institute of Technology Delhi. I obtained my Ph.D. in quantum gravity from the Indian Institute of Science Education and Research Mohali under the supervision of Prof. Kinjalk Lochan. My research lies at the intersection of quantum theory and gravitation, exploring fundamental questions that arise when these two pillars of modern physics meet.

Here’s a glimpse into some of my recent research highlights.

<!-- BEGIN SLIDESHOW SECTION -->
<section class="slideshow-wrapper">
<!-- Slideshow CSS -->
<style>
.slideshow-container {
  position: relative;
  max-width: 100%;
  margin: 2rem auto;
}

.slideshow-container .slide {
  display: none;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  margin: auto;
  text-align: center;  /* Optional: helps with captions */
}

.slideshow-container .slide-images {
  display: flex;
  justify-content: center;
  flex-wrap: wrap;
  gap: 10px;
}

.slideshow-container .slide-images img {
  width: 45%;
  border-radius: 6px;
}

.slideshow-container .caption {
  font-style: italic;
  margin-top: 0.5rem;
  text-align: center;
  font-size: 0.95rem; 
  max-width: 90%;
  margin-left: auto;
  margin-right: auto;
}

.slideshow-container .prev, .next {
  cursor: pointer;
  position: absolute;
  top: 45%;
  padding: 10px;
  color: black;
  font-weight: bold;
  font-size: 18px;
  background: rgba(240,240,240,0.8);
  border-radius: 4px;
  user-select: none;
  z-index: 2;
}
.slideshow-container .prev:hover, .next:hover {
  background: #ccc;
}
.slideshow-container .prev { left: 0; }
.slideshow-container .next { right: 0; }

.slideshow-container .dots {
  text-align: center;
  margin-top: 1rem;
}
.slideshow-container .dot {
  cursor: pointer;
  height: 12px;
  width: 12px;
  margin: 0 4px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.3s;
}
.slideshow-container .dot.active {
  background-color: #333;
}

@media screen and (max-width: 600px) {
  .caption {
    font-size: 0.8rem !important;
  }

  .slide-images img {
    width: 90% !important;
  }
}

</style>

<div class="slideshow-container" id="slideshow">

  <div class="slide">
    <div class="slide-images">
      <img src="/images/contour_plot_A=5.0.png" alt="Field Correlation" />
      <img src="/images/contour_plot_A=5.0_m.png" alt="Momentum Correlation" />
    </div>
    <div class="caption">
      Quantum correlations of a test field propagating in a spacetime undergoing critical collapse, evaluated at the end of the numerical simulation. Dashed black lines = areal radius of apparent horizon, red dashed lines = location of apparent horizon. Top: field correlation, Bottom: momentum correlation.
    </div>
  </div>
  
  <div class="slide" style="display: flex;">
    <div class="slide-images">
      <img src="/images/QC1.png" alt="QC1" />
      <img src="/images/QC2.png" alt="QC2" />
    </div>
    <div class="caption">
      The quantum dynamics of the FLRW universe with dust and a positive cosmological constant depicting quantum. Heatmap shows the probability distribution associated with the wave packet; solid black curve = expectation value of volume, dotted = classical trajectory, dashed = uncertainty region. Top: broader Λ-distribution, Bottom: sharper Λ-distribution.
    </div>
  </div>
  
<!-- This section describes my research projects in quantum gravity -->
<!--  <div class="slide"> -->
<!--    <div class="slide-images"> -->
<!--      <img src="/images/QC3.png" alt="QC3" /> -->
<!--      <img src="/images/QC4.png" alt="QC4" /> -->
<!--    </div> -->
<!--    <div class="caption"> -->
<!--            The quantum dynamics of the FLRW universe with dust and a negative cosmological constant showing cyclic evolution. Heatmap shows the probability distribution associated with the wave packet; solid black curve = expectation value of volume, dotted = classical trajectory, dashed = uncertainty region. Top: coherent wave packet, Bottom: Gaussian wave packet with same mean Λ but sharper width. -->
<!--    </div> -->
<!--  </div> -->

  <a class="prev" onclick="plusSlides(-1)">❮ </a>
  <a class="next" onclick="plusSlides(1)"> ❯</a>

  <div class="dots">
    <span class="dot" onclick="currentSlide(0)"></span>
    <span class="dot" onclick="currentSlide(1)"></span>
  </div>
</div>

<script>
let slideIndex = 0;
let slides, dots, slideshow, timer;

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

document.addEventListener("DOMContentLoaded", function () {
  slides = document.querySelectorAll(".slide");
  dots = document.querySelectorAll(".dot");
  slideshow = document.getElementById("slideshow");

  slideshow.addEventListener("mouseenter", pauseAutoSlide);
  slideshow.addEventListener("mouseleave", startAutoSlide);

  showSlide(slideIndex);
  startAutoSlide();
});
</script>

</section>
<!-- END SLIDESHOW SECTION -->


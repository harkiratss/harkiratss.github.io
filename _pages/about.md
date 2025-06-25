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
.slideshow {
  max-width: 100%;
  margin: 2rem auto;
  position: relative;
}
.slide {
  display: none;
}
.slide img {
  width: 48%;
  margin: 0 1%;
  vertical-align: top;
}
.caption {
  font-style: italic;
  margin-top: 0.5rem;
  text-align: center;
  font-size: 0.95rem;
}
</style>

<!-- Slideshow HTML -->
<div class="slideshow">
  <div class="slide" style="display:block;">
    <img src="/images/QC1.png" />
    <img src="/images/QC2.png" />
    <div class="caption">
      The quantum dynamics of the FLRW universe with dust and a positive cosmological constant depicting quantum. Heatmap shows the probability distribution associated with the wave packet; solid black curve = expectation value of volume, dotted = classical trajectory, dashed = uncertainty region. Top: broader Λ-distribution, Bottom: sharper Λ-distribution.
    </div>
  </div>

  <div class="slide">
    <img src="/images/QC3.png" />
    <img src="/images/QC4.png" />
    <div class="caption">
      Results for a negative cosmological constant showing cyclic evolution. Heatmap shows the probability distribution associated with the wave packet; solid black curve = expectation value of volume, dotted = classical trajectory, dashed = uncertainty region. Top: coherent wave packet, Bottom: Gaussian wave packet with same mean Λ but sharper width.
    </div>
  </div>

  <div class="slide">
    <img src="/images/contour_plot_A=5.0.png" />
    <img src="/images/contour_plot_A=5.0_m.png" />
    <div class="caption">
      Quantum correlations of a test field propagating in a spacetime undergoing critical collapse, evaluated at the end of the numerical simulation. Dashed black lines = areal radius of apparent horizon, red dashed lines = location of apparent horizon. Top: field correlation, Bottom: momentum correlation.
    </div>
  </div>
</div>

<!-- JavaScript for slideshow -->
<script>
let slideIndex = 0;
const slides = document.querySelectorAll(".slide");

function showSlides() {
  slides.forEach(s => s.style.display = "none");
  slideIndex = (slideIndex + 1) % slides.length;
  slides[slideIndex].style.display = "block";
}
setInterval(showSlides, 5000); // 5 seconds per slide
</script>

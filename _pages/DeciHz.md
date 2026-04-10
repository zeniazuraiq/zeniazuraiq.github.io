---
layout: page
permalink: /CGW_DeciHz_CSCStars
nav: false
nav_order: 5
---

<style>
  /* This ensures the iframe doesn't get restricted by the theme's layout */
  .fixed-plot-wrapper {
    width: 100%;
    display: flex;
    justify-content: center;
    overflow-x: auto; /* Adds a scrollbar if the screen is narrower than 1000px */
  }
</style>

<div class="l-page">
  <div class="fixed-plot-wrapper">
    <iframe 
      src="{{ '/assets/DeciHz_3d_SNR_truncated.html' | relative_url }}" 
      width="1000" 
      height="1000" 
      frameborder="0" 
      scrolling="no">
    </iframe>
  </div>
</div>
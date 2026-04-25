---
layout: page
title: Gallery 2026 (Jan - Apr)
permalink: /gallery/
description: Chronicles of the journey 
featured_image: grandcanyon.jpg
---

<style>
.orcas-gallery {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
  margin-top: 20px;
}

.orcas-gallery img {
  width: 100%;
  height: auto;
  border-radius: 4px;
  box-shadow: 0 2px 4px rgba(0,0,0,0.1);
  object-fit: cover;
  aspect-ratio: 4/3; /* Keeps the grid uniform if images have different dimensions */
}

/* Makes the gallery responsive for mobile viewing */
@media (max-width: 768px) {
  .orcas-gallery {
    grid-template-columns: repeat(2, 1fr);
  }
}
@media (max-width: 480px) {
  .orcas-gallery {
    grid-template-columns: 1fr;
  }
}
</style>

<div class="orcas-gallery">
  {% for i in (1..49) %}
    {% assign num = i | prepend: '00' | slice: -2, 2 %}
    <img src="{{ site.baseurl }}/images/04-26/{{ num }}-498-orcas-{{ num }}.jpg" alt="Orcas Street Property Renovation in Morro Bay - Photo {{ num }}" loading="lazy">
  {% endfor %}
</div>
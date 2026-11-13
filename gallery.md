---
layout: page
title: Gallery 2026
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

<h2>Fall 2026</h2>
<div class="orcas-gallery">
  {% assign fall = "2026-10-orcas-rough-in.jpg,2026-10-orcas-insulation-wide.jpg,2026-10-orcas-bathroom-drywall.jpg,2026-10-orcas-drywall-corner-window.jpg,2026-10-orcas-drywall-upstairs-ocean-view.jpg,2026-10-orcas-front-scaffold.jpg,2026-10-orcas-interior-white-walls.jpg,2026-10-orcas-shower-backer-board.jpg,2026-11-orcas-kitchen-cabinets.jpg,2026-11-orcas-living-room-flooring.jpg,2026-11-orcas-purple-door-paint.jpg,2026-11-orcas-landscaping.jpg" | split: "," %}
  {% for file in fall %}
    <img src="{{ site.baseurl }}/images/posts/{{ file }}" alt="498 Orcas Street Renovation in Morro Bay - Fall 2026" loading="lazy">
  {% endfor %}
</div>

<h2>Summer 2026</h2>
<div class="orcas-gallery">
  {% assign summer = "orca-exterior-36-36.jpg,orca-exterior-38-38.jpg,orca-exterior-40-40.jpg,orca-exterior-41-41.jpg,orca-exterior-42-42.jpg,orca-exterior-44-44.jpg,orca-exterior-46-46.jpg,orca-exterior-48-48.jpg,lumber-delivery.jpg,siding-scaffold.jpg,sun-scaffold.jpg,progress-street-view.jpg,interior-demo-bath-1.jpg,interior-demo-bath-2.jpg" | split: "," %}
  {% for file in summer %}
    <img src="{{ site.baseurl }}/images/07-26/{{ file }}" alt="498 Orcas Street Renovation in Morro Bay - Summer 2026" loading="lazy">
  {% endfor %}
</div>

<h2>January &ndash; April 2026</h2>
<div class="orcas-gallery">
  {% assign spring = "01,02,05,07,09,10,14,19,20,21,25,30,32,35,36,37,38,39,41,42,43,44,46,48,49,50,51,52,53,54" | split: "," %}
  {% for num in spring %}
    <img src="{{ site.baseurl }}/images/04-26/{{ num }}-498-orcas-{{ num }}.jpg" alt="Orcas Street Property Renovation in Morro Bay - Photo {{ num }}" loading="lazy">
  {% endfor %}
</div>
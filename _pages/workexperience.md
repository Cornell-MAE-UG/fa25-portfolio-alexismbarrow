---
layout: default
title: Work Experience
permalink: /workexperience/
---

<div class="gallery-container">
<div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
       <a href="{{ '/workexperience/cev/' | relative_url }}">
          <img src="{{ '/assets/images/cev-thumb.png' | relative_url }}" alt="Cornell Electric Vehicles" />
          <p>Cornell Electric Vehicles</p>
        </a>
      </div>
    {% endfor %}
</div>
</div>
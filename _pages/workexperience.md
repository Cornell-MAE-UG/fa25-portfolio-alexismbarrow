---
layout: default
title: Work Experience
permalink: /workexperience/
---
picms

<div class="gallery-container">
<div class="project-gallery">
    {% for project in site.projects %}
      <div class="gallery-item">
       <a href="{{ '/workexperience/cev/' | relative_url }}">
          <img src="{{ '/assets/images/cev-thumb.png' | relative_url }}" alt="CEV" />
          <p>CEV</p>
        </a>
      </div>
    {% endfor %}
</div>
</div>
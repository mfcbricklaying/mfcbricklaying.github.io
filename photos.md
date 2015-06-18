---
layout: page
title_nav: Photos
title: Photos
permalink: /photos/
weight: 3
enabled: true
---

<div class="row">
			<div id="try"></div>
			<ul id="box-container">
        {% assign photo_base_url = site.photos_base_url %}
        {% for photo in site.data.photos %}
        <div class="col-xs-8 col-md-4">
          <li class="box">
            <a href="{{ photo_base_url }}/{{ photo.file_name }}" class="swipebox" title="{{ photo.title : photo.title ? photo.file_name }}">
              <img src="{{ photo_base_url }}/{{ photo.file_name }}" alt="{{ photo.file_name }}" class="img-responsive">
            </a>
          </li>
        </div>
        {% endfor %}
			</ul>
</div>

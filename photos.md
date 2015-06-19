---
layout: page
title_nav: Photos
title: Photos
permalink: /photos/
weight: 3
enabled: true
---

<p>Below are some photos of prior work completed by MFC Bricklaying.
To view a photo, simply click on it and a larger version will be displayed.<br /><br />
You can use the arrow keys to navigate through the photos, or swipe left/right on a mobile device.
</p><br />

<div class="row center-block">
			<div id="try"></div>
			<ul id="box-container">
        {% assign photo_base_url = site.photos.base_url %}
        {% for photo in site.data.photos %}
        <div class="{{ site.photos.mobile.col_style }} {{ site.photos.desktop.col_style }}">
          <li class="box">
            <a href="{{ photo_base_url }}/{{ photo.file_name }}" class="swipebox" title="{{ photo.title : photo.title ? photo.file_name }}">
              <img src="{{ photo_base_url }}/{{ photo.file_name }}" alt="{{ photo.file_name }}" class="img-responsive">
            </a>
          </li>
        </div>
        {% endfor %}
			</ul>
</div>

---
title: Cover design case
subtitle: Lorem ipsum dolor sit amet, consetetur sadipscing tempor invidunt ut labore et dolore magna aliquyam erat, sed diam voluptua.
image: thumb-olia-gozha.jpg
topics: [Covers]
navbar:
  sticky: false
  transparent: true
  transparent_color: light
header:
  layout: center # Options: center 1-2 or 2-3
  background_image: alisha-hieb.jpg
  background_overlay: "rgba(0, 0, 0, 0.7)"
  color: light
  section_size: xlarge
  parallax: true
---

{% include block.html 
	width="2-3"
  block="content-post3"
  section_size="small"
  section_container="small"
%}

{% include block.html 
	width="2-3"
  block="content-post"
  section_size="small"
  section_container="small"
%}

{% include gallery.html 
	cols="3"
	gallery="portfolio-1"
	caption="true"
	lightbox="true"
  section_size="small"
%}

{% include block.html 
	width="2-3"
  block="content-post2"
  section_size="small"
  section_container="small"
%}

{% include image.html 
	img="alexander-read.jpg"
  section_size="small"
%}
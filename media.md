---
title: Media
subtitle: Show off your images and videos, the options and posibilities are endless.
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: center # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image: header-3.jpeg
  background_overlay: "rgba(0, 0, 0, 0.45)"
  color: light
  section_size: xlarge
  heading_size: large
  parallax: true
---

{% include content.html 
  block="content-image"
  section_size="large"
  section_title="Images aligned in content"
  section_padding="remove-bottom"
  section_container="xsmall"
  section_align="center"
%}

{% include image.html 
	src="alexander-read.jpg"
  alt="Alt for image"
  section_size="large"
  section_padding="remove-bottom"
  section_title="Image in lightbox"
  section_align="center"
  section_container="small"
  lightbox="true"
%}

{% include gallery.html 
  section_size="large"
  section_padding="remove-bottom"
  section_title="Image Gallery Lightbox" 
  section_align="center"
  cols="3"
  gallery="gallery-1"
  caption="true"
  lightbox="true"
%}

{% include slider.html 
  section_size="large"
  section_padding="remove-bottom"
  section_title="Image Slider" 
  section_align="center"
  section_container="xsmall"
  color="light"
  block="slider-home" 
  grid="1-1"
  gutter="false"
%}

{% include slider.html 
  block="slider-home" 
  section_size="large"
  section_padding="remove-bottom"
  section_align="center" 
  section_title="Cards in slider" 
  content_align="center"
  color="light"
  autoplay="true"
  sets="true"
  grid="1-3"
  navigation="outside"
  dotnav="true"
%}

{% include instagram.html 
  section_size="large"
  section_padding="remove-bottom"
  section_container="default"
  section_title="Instagram Images"
  section_align="center"
  cols="4" 
  count="8" 
  gutter="small"
%}

{% include content.html 
  block="videos"
  section_size="large"
  section_title="Responsive videos" 
  section_container="xsmall"
  section_align="center"
%}

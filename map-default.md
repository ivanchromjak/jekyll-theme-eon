---
title: Map Default
width: full
navbar:
  transparent: true
  transparent_color: light
header:
  layout: center # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image: https://source.unsplash.com/A5rCN8626Ck/1800x700
  background_overlay: "rgba(0, 0, 0, 0.45)"
  color: light
  section_size: xlarge
  heading_size: medium
  parallax: true
---

{% include content.html 
  block="content-post2"
  section_container="xsmall"
  section_size="medium"
%}

{% include map.html 
  latitude="19.419897" 
  longitude="-99.164967" 
  zoom="12" 
  section_size="medium"
  section_padding="remove-top"
  section_container="small"
  height="large"
%}

{% include content.html 
  block="content-post2"
  section_container="xsmall"
  section_size="medium"
  section_padding="remove-top"
%}
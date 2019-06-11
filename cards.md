---
title: Cards
subtitle: The options and posibilities are endless
layout: full
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: center # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image: Working-Space.jpg
  background_overlay: "linear-gradient(to right bottom,rgba(28, 54, 191, 0.85) 15%,rgba(27, 51, 191, 0.8) 50%,rgba(67, 27, 191, 0.8) 80%)"
  color: light
  section_size: large
  heading_size: medium
  parallax: true
---

{% include cards.html 
  block="card-media-11" 
  media="left" 
  section_size="medium"
  background_color="default"
  section_title="Cards with images"
  section_align="center"
%}

{% include cards.html 
  block="card-media-12" 
  media="right" 
  section_size="medium"
  background_color="default"
  card_style="default"
%}

{% include cards.html 
  block="card-media-21" 
  media="left" 
  section_size="medium"
  background_color="default"
  card_style="secondary"
%}

{% include cards.html 
  block="card-media-22" 
  media="right" 
  section_size="medium"
  background_color="default"
  card_style="primary"
%}

{% include cards.html 
  block="card-media" 
  media="top" 
  section_size="medium"
  section_container="expand"
  background_color="default"
  card_style="default"
  content_align="center"
%}

{% include cards.html 
  block="card-media-1" 
  media="top" 
  section_size="medium"
  section_container="small"
  background_color="default"
  card_style="secondary"
%}

{% include cards.html 
  block="card-media-2" 
  media="top" 
  section_size="medium"
  section_container="xsmall"
  background_color="default"
  card_style="primary"
  content_align="center"
%}

{% include cards.html 
  block="feature-1" 
  media="top" 
  section_size="medium"
  section_title="Cards with SVG icons"
  section_align="center"
  background_color="muted"
  content_align="center"
  grid="1-4"
%}

{% include cards.html 
  block="feature-2" 
  media="top" 
  section_size="medium"
  background_color="muted"
  content_align="center"
  card_style="default"
  grid="1-4"
%}

{% include cards.html 
  block="feature-3" 
  media="left" 
  section_size="medium"
  background_color="muted"
  card_style="secondary"
  grid="1-2"
%}

{% include cards.html 
  block="feature-4" 
  media="right" 
  section_size="medium"
  background_color="muted"
  content_align="right"
  card_style="primary"
  grid="1-2"
%}

{% include slider.html 
  block="feature" 
  media="top" 
  background_color="default"
  section_size="medium"
  section_align="center" 
  section_title="Cards in slider" 
  content_align="center"
  autoplay="true"
  sets="true"
  grid="1-4"
  navigation="outside"
  dotnav="true"
%}

{% include slider.html 
  background_color="default"
  block="card-media" 
  media="top" 
  section_size="medium"
  content_align="center"
  section_container="small"
  card_style="default"
  navigation="outside"
  grid="1-2"
%}

{% include slider.html 
  block="feature" 
  media="left" 
  background_color="default"
  section_size="medium"
  card_style="secondary"
  grid="1-2"
%}

{% include cards.html 
  block="pricing" 
  section_size="medium"
  section_container="small"
  background_color="muted" 
  content_align="center"
%}

{% include cards.html 
  block="pricing" 
  section_size="medium"
  section_title="Pricing Cards" 
  section_align="center"
  background_color="muted" 
  content_align="center"
  card_style="default"
%}

{% include cards.html 
  block="pricing" 
  section_size="medium"
  background_color="muted" 
  content_align="center"
  card_style="secondary"
%}


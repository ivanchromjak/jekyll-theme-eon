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
  block="card-media-1" 
  media="left" 
  section_size="medium"
  background_color="default"
  section_title="Cards with images"
  section_align="center"
%}

{% include cards.html 
  block="card-media-2" 
  media="right" 
  section_size="medium"
  background_color="muted"
%}

{% include cards.html 
  block="card-media-3" 
  media="left" 
  section_size="medium"
  background_color="default"
  card_style="default"
%}

{% include cards.html 
  block="card-media-4" 
  media="right" 
  section_size="medium"
  background_color="secondary"
  card_style="default"
%}

{% include cards.html 
  block="card-media-1" 
  media="left" 
  section_size="medium"
  background_color="primary"
  card_style="default"
%}

{% include cards.html 
  block="card-media-2" 
  media="right" 
  section_size="medium"
  background_color="default"
  card_style="secondary"
%}

{% include cards.html 
  block="card-media-3" 
  media="right" 
  section_size="medium"
  background_color="muted"
  card_style="primary"
%}

{% include cards.html 
  block="card-media" 
  media="top" 
  section_size="medium"
  section_container="expand"
  background_color="default"
  gutter="small"
%}

{% include cards.html 
  block="card-media" 
  media="top" 
  section_size="medium"
  section_container="small"
  section_title="Two columns in small container"
  section_align="center"
  background_color="muted"
  content_align="center"
  card_style="default"
  grid="1-2"
%}

{% include cards.html 
  block="feature-1" 
  media="top" 
  section_size="medium"
  section_title="Cards with SVG icons"
  section_align="center"
  background_color="default"
  content_align="center"
  card_style="primary"
  grid="1-4"
%}

{% include cards.html 
  block="feature-2" 
  media="left" 
  section_size="medium"
  section_title="Cards with left aligned icons"
  section_align="center"
  background_color="muted"
  content_align="left"
  card_style="secondary"
  grid="1-2"
%}

{% include cards.html 
  block="feature-3" 
  media="right" 
  section_size="medium"
  section_title="Cards with right aligned icons"
  section_align="center"
  background_color="default"
  content_align="left"
  card_style="default"
  grid="1-3"
%}

{% include cards.html 
  block="feature" 
  media="top" 
  section_size="medium"
  section_title="Cards with right aligned icons"
  section_align="center"
  background_color="muted"
  content_align="center"
  grid="1-4"
  gutter="large"
%}

{% include cards.html 
  block="feature" 
  media="left" 
  section_size="medium"
  section_title="Cards with right aligned icons"
  section_align="center"
  background_color="muted"
  content_align="left"
  grid="1-4"
  gutter="large"
%}

{% include cards.html 
  block="feature" 
  media="right" 
  section_size="medium"
  section_title="Cards with right aligned icons"
  section_align="center"
  background_color="muted"
  content_align="left"
  grid="1-4"
  gutter="large"
%}

{% include slider.html 
  block="feature" 
  layout="card-top" 
  section_size="large"
  section_align="center" 
  section_title="Slider" 
  content_align="center"
  autoplay="true"
  sets="true"
  card_style="default"
  grid="1-3"
  dotnav="true"
%}

{% include slider.html 
  block="feature" 
  layout="card-top" 
  background_color="muted"
  section_size="large"
  section_align="center" 
  section_title="Slider" 
  content_align="center"
  autoplay="true"
  sets="true"
  card_style="primary"
  grid="1-4"
  navigation="outside"
  dotnav="true"
%}

{% include slider.html 
  background_color="rgb(247, 234, 222)"
  block="card-media" 
  layout="card-top" 
  section_size="large"
  section_align="center" 
  section_title="Slider" 
  section_subtitle="Slider" 
  section_container="expand"
  content_align="center"
  autoplay="true"
  card_style="secondary"
  grid="1-4"
%}

{% include cards.html 
  block="pricing" 
  section_size="large"
  section_title="Pricing Cards" 
  section_align="center"
  background_color="muted" 
  card_style="default"
  align="center"
%}
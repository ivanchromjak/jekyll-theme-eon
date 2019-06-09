---
title: Cards
subtitle: Donec porttitor semper lacus, et posuere arcu varius rutrum mollis vestibulum diam ac congue
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
  block="home-card-2" 
  media="left" 
  section_size="large"
  background_color="muted"
%}

{% include cards.html 
  block="home-card-1" 
  media="right" 
  section_size="large"
  section_padding="remove-top"
  background_color="muted"
%}

{% include cards.html 
  block="home-card-3" 
  media="left" 
  section_size="large"
  background_color="#1B33BF"
  style="default"
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
  style="default"
  grid="1-3"
  dotnav="true"
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
  style="primary"
  grid="1-4"
  navigation="outside"
  dotnav="true"
%}

{% include slider.html 
  background_image="https://source.unsplash.com/WHWYBmtn3_0/1600x900"
  background_overlay="rgba(0, 0, 0, 0.5)"
  block="home-card" 
  layout="card-top" 
  section_size="large"
  section_align="center" 
  section_title="Slider" 
  section_subtitle="Slider" 
  content_align="center"
  autoplay="true"
  style="secondary"
  grid="1-3"
%}

{% include cards.html 
  block="pricing" 
  section_size="large"
  section_title="Pricing Cards" 
  section_align="center"
  background_color="muted" 
  style="default"
  align="center"
%}
---
title: Some title
subtitle: Some subbbbtitle
layout: full
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: 1-1 # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  # background_color: "#1B33BF"
  background_image: BlackLavaField.jpg
  background_video: BlackLavaField.mp4
  # background_align: center-center
  background_overlay: "rgba(27, 51, 191, 0.4)" #"rgba(0, 0, 0, 0.35)" #"rgba(5, 15, 140, 0.75)"
  color: light
  # header_size: large
  heading_size: large
  height: full
  parallax: true
  container:
    block: header-home
    # title: false
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include cards.html 
    block="feature" 
    section_background="default" 
    section_size="large"
    section_title="The first trully multipurpose Jekyll theme" 
    section_subtitle="Loaded with awesome features and options to design your perfect site"
    section_header_align="center"
    section_content_align="center"
    media="top"
    grid="1-4"
  %}

  {% include cards.html 
    block="home-why" 
    section_title="Why use Eon theme?"
    section_header_align="center"
    section_size="large"
    section_color="light"
    section_background="primary"
    media="top" 
    section_content_align="left"
    grid="1-3"
  %}

  {% include video.html 
    block="video-intro" 
    section_background="default" 
    section_size="large"
    section_header_align="center" 
    section_container="small"
  %}

  {% include blog.html 
    section_size="large"
    section_title="Latest Posts" 
    section_header_align="center"
    section_background="muted" 
    style="default" 
    media="top" 
    section_content_align="left"
    grid="1-3"
    count="3"
    view_all="blog/"
  %}

  {% include cards.html 
    block="pricing" 
    section_size="large"
    section_title="Pricing Cards" 
    section_header_align="center"
    section_background="muted" 
    style="default"
    align="center"
  %}

  {% include videos.html 
    block="video-home" 
    columns="3" 
    section_size="large"
    section_header_align="center"
    section_title="Video Tutorials" 
    section_subtitle="Watch screencasts to get you started fast with Jekyll" 
  %}



  {% include portfolio.html 
    section_size="large"
    section_title="Portfolio" 
    section_header_align="center"
    section_background="muted"
    cols="3"
  %}

  {% include cards.html 
    block="home-card-2" 
    media="left" 
    section_size="large"
    section="muted" 
    section_header_align="center"  
    section_content_align="left"
    center="true-"
  %}

  {% include cards.html 
    block="home-card-1" 
    media="right" 
    section_size="large"
    section="muted" 
    section_header_align="center"  
    section_background="muted"
    section_content_align="left"
    center="true-"
  %}

  {% include gallery.html 
    section_size="large"
    section_title="Image Gallery" 
    section_header_align="center"
    section_background="default"
    cols="3"
    gutter="true"
    gallery="gallery-1"
    caption="true"
    lightbox="true"
  %}

  {% include slider.html 
    section_container="none"
    block="slider-home" 
    color="light" 
    display_title="true"
  %}

  {% include map.html 
    section_container="none"
    latitude="19.4230622" 
    longitude="-99.1583328" 
    zoom="16" 
  %}

  {% include cta.html 
    section_title="Create your website today!" 
    button_style="primary" 
    button_text="Purchase" 
    button_url="https://www.envato.com" 
    section_subtitle="Experience the advatages of running a static Jekyll site and concentrate an what is important."
    blank="true" 
    section_size="large"
    section_header_align="center"
    section_image="mouse.jpg"
    section_video="mouse.mp4"
    section_overlay="rgba(0, 0, 0, 0.8)"
    section_container="small"
    section_color="#fff"
    section_content_align="center"
    layout="center"
  %}
  
  {% include team.html 
    authors="evan, john, sara, alex, tom, daniel" 
    section_title="We are here to help" 
    section_subtitle="Our team is just an email away ready to answer your questions" 
    section_header_align="center"
    section_size="large"
    section_background="muted" 
  %}

  {% include instagram.html 
    cols="4" 
    count="4" 
    gutter="false"
  %}
{% else %}

  {% include cards.html id="home-right" style="" media="right" section="muted" %}

  {% include cards.html id="home-next" style="primary" align="center" section="muted" %}

  {% include instagram.html count="8" section="default" %}

{% endif %}



<!--
background-image: linear-gradient(to right, #0acffe 0%, #495aff 100%);
background-image: linear-gradient(-225deg, #AC32E4 0%, #7918F2 48%, #4801FF 100%);
background-image: linear-gradient(-225deg, #A445B2 0%, #D41872 52%, #FF0066 100%); -->

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
  background_image: Working-Space.jpg
  background_video: Working-Space.mp4
  # background_align: center-center
  background_overlay: "linear-gradient(to right bottom,rgba(28, 54, 191, 0.85) 15%,rgba(27, 51, 191, 0.8) 50%,rgba(67, 27, 191, 0.8) 80%)"
  color: light
  # section_size: large
  heading_size: medium
  height: full
  parallax: true
  container:
    block: header-home
    # title: false
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include features.html 
    block="feature" 
    background_color="default" 
    section_size="large"
    section_title="The first multipurpose Jekyll theme" 
    section_align="center"
    content_align="center"
    media="top"
    grid="1-4"
  %}

  {% include features.html 
    block="home-why" 
    section_title="Why use Eon theme?"
    section_align="center"
    section_size="large"
    section_color="light-"
    background_color="muted"
    media="top" 
    content_align="left"
    grid="1-3"
  %}

  {% include cta.html 
    section_title="Create your website today!" 
    button_style="danger" 
    button_text="Purchase" 
    button_url="https://www.envato.com" 
    section_subtitle="Experience the advatages of running a static Jekyll site and concentrate an what is important."
    blank="true" 
    section_size="large"
    section_align="center"
    background_image="https://source.unsplash.com/WHWYBmtn3_0/1600x900"
    background_overlay="rgba(0, 0, 0, 0.5)"
    section_container="small"
    section_color="#fff"
    content_align="center"
    layout="center"
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

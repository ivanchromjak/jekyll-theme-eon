---
layout: full
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: center # Options: center 1-2 or 2-3
  # background_color: "#1B33BF"
  background_image: sand.jpg
  background_video: sand.mp4
  # background_align: center-center
  background_overlay: "rgba(5, 15, 140, 0.9)"
  color: light
  # section_size: large
  height: full
  parallax: true
  container:
    block: header-home-2
    # title: false
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include features.html 
    block="feature" 
    background_color="default" 
    section_title="The first trully multipurpose Jekyll theme" 
    section_subtitle="Theme is loaded with awesome features and countless options giving you the flexibility to design your perfect site"
    section_align="center"
    content_align="center"
    media="top"
    grid="1-4"
  %}

  {% include features.html 
    block="home-why-jekyll" 
    section_title="Why switch to Jekyll"
    section_align="center"
    section_size="large"
    section_color="light"
    background_color="primary"
    media="top" 
    content_align="left"
    grid="1-3"
  %}

  {% include faqs.html 
    background_color="default"
    multiple="true" 
    section_size="large"
    section_title="Frequently asked questions" 
    section_container="small"
    section_align="center"
    content_align="left"
    category="presale" 
    section_subtitle="Find quicke answers to frequent pre-sale questions asked by customers" 
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
    background_image="mouse.jpg"
    background_video="mouse.mp4"
    background_overlay="rgba(0, 0, 0, 0.86)"
    section_container="small"
    section_color="#fff"
    content_align="center"
    layout="center"
  %}
  
  {% include team.html 
    authors="evan, john, sara, alex, tom, daniel" 
    section_title="We are here to help" 
    section_subtitle="Our team is just an email away ready to answer your questions" 
    section_align="center"
    section_size="large"
    background_color="muted" 
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

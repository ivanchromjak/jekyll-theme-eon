---
layout: full
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
header:
  layout: center # Options: center 1-2 or 2-3
  # background_image: bg1.jpg
  # background_align: center-center
  # background_overlay: "rgba(255, 255, 255, 0.7)"
  section_size: 
  parallax: true
  container:
    block: header-home-2
    # title: false
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include features.html 
    block="home-why-jekyll" 
    section_title="Why switch to Jekyll"
    section_align="center"
    section_size="large"
    background_color="primary"
    media="top" 
    content_align="left"
    grid="1-3"
  %}

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

  {% include block.html id="support" section="default" type="center" padding="remove-bottom" %}

  {% include cta.html 
    title="Create your new website today!" button_style="danger" button_text="Join Us" button_url="https://www.envato.com" 
    subtitle="Experience the advatages of static Jekyll site and piece of mind."
    blank="true" 
    section_size="xlarge"
    background_image="multipurpose.webp"
    background_overlay="rgba(255, 255, 255, 0.8)"
    section_container="small"
    content_align="center"
    layout="center"
  %}

  {% include faqs.html 
    background_color="muted"
    multiple="true" 
    section_title="Frequently asked questions" 
    section_container="small"
    category="presale" 
    section_subtitle="Find quicke answers to frequent pre-sale questions asked by customers" 
  %}

  {% include team.html authors="evan, john, sara, alex, tom, daniel" title="We are here to help" subtitle="Our team is just an email away ready to answer your questions" %}

  {% include cta.html 
    section_align="center"
    section_container="small"
    layout="center"
    background_color="primary"
    title="Support continuous development of this theme with your contribution" 
    button_text="Purchase" 
    button_url="https://www.paypal.me/ivanchromjak" 
    blank="true" 
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

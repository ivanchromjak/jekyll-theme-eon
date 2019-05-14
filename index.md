---
layout: full
width: full
navbar:
  sticky: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: center # Options: center 1-2 or 2-3
  height: full-
  background_image: header-home.jpg
  background_align: bottom-center
  background_color: "#000"
  background_video: https://app.coverr.co/s3/mp4/Feet-and-Sand.mp4
  background_overlay: "linear-gradient(to right bottom,rgba(12, 180, 206, 0.85) 5%,rgba(0, 108, 255, 0.85) 30%,rgba(144, 18, 254, 0.85) 80%)"
  color: light
  container:
    block: header-home-container
    # title: false
  container-2:
    block: header-home-container-2
    title: false
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include section-content.html 
    block="content-post"
    section_size="large"
    section_padding="remove-vertical-"
    section_height="viewport-"
    section_light="true"
    section_container="small"
    section_title="This is section title"
    section_subtitle="This is section subtitle"
    section_align="center"
    background_color="primary-"
    background_image="sand.jpg"
    background_video=""
    background_align="top-left"
    background_overlay="linear-gradient(to right bottom,rgba(12, 180, 206, 0.85) 5%,rgba(0, 108, 255, 0.85) 30%,rgba(144, 18, 254, 0.85) 80%)"
    align="center" 
  %}

  {% include section-cards.html 
    block="home-why" 
    section_title="Why switch to Jekyll" 
    section_align="center"
    background_color="muted" 
    style="default" 
    media="top" 
    content_align="left"
    grid="1-4"
  %}

  {% include section-cards.html 
    block="home-cta" 
    section_title="Why switch to Jekyll" 
    section_align="center"
    background_color="default" 
    style="default" 
    media="top" 
    content_align="left"
    grid="1-3"
  %}

  {% include section-features.html 
    block="feature" 
    background_color="muted" 
    align="center" 
    section_title="Awesome Features" 
    section_align="center"
    content_align="left"
  %}

  {% include section-cards.html 
    block="pricing" 
    section_title="Pricing" 
    section_align="center"
    background_color="primary" 
    style="default"
    align="center"
  %}


  {% include block.html id="support" section="default" type="center" padding="remove-bottom" %}

  {% include cta.html title="Support continuous development of this theme with your contribution" button_style="danger" button_text="Support Us" button_url="https://www.paypal.me/ivanchromjak" blank="true" section="secondary" %}

  {% include videos.html id="video" columns="3" title="Video Tutorials" subtitle="Watch screencasts to get you started fast with Jekyll" %}

  {% include faqs.html multiple="true" title="Frequently asked questions" category="presale" subtitle="Find quicke answers to frequent pre-sale questions asked by customers" %}

  {% include video.html id="video-home2" section="primary" layout="center" %}

  {% include portfolio.html topic="Service" section="muted" layout="" %}

  {% include portfolio.html section="muted" layout="" %}

  {% include video.html id="video-home3" section="default" layout="" %}

  {% include cta.html title="Support continuous development of this theme with your contribution" button_text="Support Us" button_url="https://www.paypal.me/ivanchromjak" blank="true" section="muted" align="center" %}

  {% include cta.html title="Support continuous development of this theme with your contribution" button_text="Support Us" button_url="https://www.paypal.me/ivanchromjak" blank="true" %}

  {% include map.html latitude="41.449689" longitude="-81.639102" zoom="16" %}

  {% include slider.html id="feature" layout="card-top" section="muted" align="center" title="Slider" 
    center="true"
    autoplay="true"
    sets="true"
  %}

  {% include slider.html id="home-cta" color="light" %}

{% else %}

  {% include section-cards.html id="home-right" style="" media="right" section="muted" %}

  {% include section-cards.html id="home-next" style="primary" align="center" section="muted" %}

  {% include instagram.html count="8" section="default" %}

{% endif %}

{% include team.html authors="evan, john, sara, alex, tom, daniel" title="We are here to help" subtitle="Our team is just an email away ready to answer your questions" %}


<!--
background-image: linear-gradient(to right, #0acffe 0%, #495aff 100%);
background-image: linear-gradient(-225deg, #AC32E4 0%, #7918F2 48%, #4801FF 100%);
background-image: linear-gradient(-225deg, #A445B2 0%, #D41872 52%, #FF0066 100%); -->

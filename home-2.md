---
layout: full
width: full
navbar:
  sticky: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: 2-3 # Options: center 1-2 or 2-3
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

  {% include block.html 
    block="content-post"
    section_size="large"
    section_padding="remove-vertical-"
    section_height="viewport-"
    section_color="light"
    section_container="small"
    section_title="This is section title"
    section_subtitle="This is section subtitle"
    section_header_align="center"
    section_image="sand.jpg"
    section_video=""
    background_align="top-left"
    section_overlay="linear-gradient(to right bottom,rgba(12, 180, 206, 0.85) 5%,rgba(0, 108, 255, 0.85) 30%,rgba(144, 18, 254, 0.85) 80%)"
    align="center" 
  %}

  {% include cards.html 
    block="home-why" 
    section_title="This is section title"
    section_subtitle="This is section subtitle"
    section_color="red"
    section_header_align="center"
    section_size="large"
    background_overlay1="rgba(255, 255, 255, 0.73)"
    section_background="#563493"
    style="default" 
    media="top" 
    section_content_align="center"
    grid="1-4"
  %}

  {% include cards.html 
    block="home-cta" 
    section_title="Why switch to Jekyll" 
    section_header_align="center"
    section_background="default" 
    style="default" 
    media="top" 
    section_content_align="left"
    grid="1-3"
  %}

  {% include cards.html 
    block="feature" 
    section_background="muted" 
    section_title="Awesome Features" 
    section_header_align="center"
    section_content_align="center"
    media="top"
    grid="1-3"
  %}

  {% include cards.html 
    block="feature-6" 
    section_background="default" 
    media="left"
    grid="1-1"
  %}

  {% include cards.html 
    block="feature-6" 
    section_background="primary" 
    media="right"
    grid="1-1"
  %}

  {% include cards.html 
    block="pricing" 
    section_title="Pricing" 
    section_header_align="center"
    section_background="muted" 
    style="default"
    align="center"
  %}

  {% include cta.html 
    title="Create your new website today!" button_style="danger" button_text="Join Us" button_url="https://www.envato.com" 
    subtitle="Experience the advatages of static Jekyll site and piece of mind."
    blank="true" 
    section_size="xlarge"
    section_image="multipurpose.webp"
    section_overlay="rgba(0, 0, 0, 0.8)"
    section_container="small"
    section_content_align="center"
    section_content_color="light"
    layout="center"
  %}

  {% include cta.html 
    title="Create your new website today!" button_style="danger" button_text="Join Us" button_url="https://www.envato.com" 
    subtitle="Experience the advatages of static Jekyll site and piece of mind."
    blank="true" 
    section_size="xlarge"
    section_image="multipurpose.webp"
    section_overlay="rgba(255, 255, 255, 0.8)"
  %}

  {% include videos.html id="video" columns="3" title="Video Tutorials" subtitle="Watch screencasts to get you started fast with Jekyll" %}


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

  {% include cards.html id="home-right" style="" media="right" section="muted" %}

  {% include cards.html id="home-next" style="primary" align="center" section="muted" %}

  {% include instagram.html count="8" section="default" %}

{% endif %}



<!--
background-image: linear-gradient(to right, #0acffe 0%, #495aff 100%);
background-image: linear-gradient(-225deg, #AC32E4 0%, #7918F2 48%, #4801FF 100%);
background-image: linear-gradient(-225deg, #A445B2 0%, #D41872 52%, #FF0066 100%); -->

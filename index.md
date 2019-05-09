---
layout: full
width: full
title: Build fast and secure websites with Jekyll
subtitle: 'Multipurpose Jekyll theme. Create company or personal site and host on GitHub for free.
          <br><br>
          <a class="uk-button uk-button-large uk-button-danger uk-box-shadow-medium hvr-up" href="https://github.com/ivanchromjak/jekyll-theme-plus/fork"><span uk-icon="github"></span> Fork on GitHub</a> &nbsp;
          <a class="uk-button uk-button-large uk-button-light uk-box-shadow-medium hvr-up" href="https://github.com/ivanchromjak/jekyll-theme-plus/fork"><span uk-icon="copy"></span> Documentation</a>'
navbar:
  sticky: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: 2-3 # Options: center 1-2 or 2-3
  height: full-
  background:
    # image: https://source.unsplash.com/aViOQZzikVs
    align: center
    color: "linear-gradient(-40deg, #0acffe 0%, #495aff 100%)"
    overlay: true
  color: light
  container:
    title: true
    subtitle: true
    search: true
    newsletter: mailchimp
    image: /assets/icons/rocket-2.svg
    slideshow: slideshow-1
    content: <iframe width="560" height="315" src="https://www.youtube.com/embed/BotpJkJ0BKE" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  container2:
    title: true
    subtitle: true
    search: true
    newsletter: mailchimp
    image: /assets/icons/rocket-2.svg
    slideshow: slideshow-1
    content: <div style="padding:56.25% 0 0 0;position:relative;"><iframe src="https://player.vimeo.com/video/333319621?title=0&byline=0&portrait=0" style="position:absolute;top:0;left:0;width:100%;height:100%;" frameborder="0" allow="autoplay; fullscreen" allowfullscreen></iframe></div><script src="https://player.vimeo.com/api/player.js"></script>
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include cards.html id="home-why" style="default" media="top" section="muted" align="center" title="Why switch to Jekyll" %}

  {% include features.html id="feature" section="default" align="center" title="Awesome Features" %}

  {% include cards.html id="pricing" style="default" section="muted" align="center" title="Pricing" %}

  {% include block.html id="support" section="default" layout="center" padding="remove-bottom" %}

  {% include cta.html title="Support continuous development of this theme with your contribution" button_style="danger" button_text="Support Us" button_url="https://www.paypal.me/ivanchromjak" blank="true" section="secondary" %}

  {% include videos.html id="video" columns="3" title="Video Tutorials" subtitle="Watch screencasts to get you started fast with Jekyll" %}

  {% include faqs.html multiple="true" title="Frequently asked questions" category="presale" subtitle="Find quicke answers to frequent pre-sale questions asked by customers" %}

  {% include video.html id="video-home2" section="primary" layout="center" %}

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

{% include team.html authors="evan, john, sara, alex, tom, daniel" title="We are here to help" subtitle="Our team is just an email away ready to answer your questions" %}


<!--
background-image: linear-gradient(to right, #0acffe 0%, #495aff 100%);
background-image: linear-gradient(-225deg, #AC32E4 0%, #7918F2 48%, #4801FF 100%);
background-image: linear-gradient(-225deg, #A445B2 0%, #D41872 52%, #FF0066 100%); -->

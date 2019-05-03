---
layout: full
width: full
title: Build fast and secure websites with Jekyll
excerpt: 'Multipurpose Jekyll theme. Create company or personal site and host on GitHub for free.
          <br><br>
          <a class="uk-button uk-button-large uk-button-danger uk-box-shadow-medium hvr-up" href="https://github.com/ivanchromjak/jekyll-theme-plus/fork"><span uk-icon="github"></span> Fork on GitHub</a> &nbsp;
          <a class="uk-button uk-button-large uk-button-light uk-box-shadow-medium hvr-up" href="https://github.com/ivanchromjak/jekyll-theme-plus/fork"><span uk-icon="copy"></span> Documentation</a>'
navbar:
  sticky: true
  animation: true
  transparent: true
  transparent_color: light
header:
    # background_image: https://source.unsplash.com/aViOQZzikVs
    background_align: center
    background_color: "linear-gradient(-40deg, #0acffe 0%, #495aff 100%)"
    background_overlay: true
    color: light
    align: left
    search: true
    height: full-
    image: /assets/icons/rocket-2.svg
---

[comment]: # (This actually is the most platform independent comment)

{% if site.template == 'base' %}

  {% include cards.html id="home-why" style="default" media="top" section="muted" align="center" title="Why switch to Jekyll" %}

  {% include features.html id="feature" section="default" align="center" title="Awesome Features" %}

  {% include cta.html title="Support continuous development of this theme with your contribution" button_style="danger" button_text="Support Us" button_url="https://www.paypal.me/ivanchromjak" blank="true" section="secondary" %}

  {% include cta.html title="Support continuous development of this theme with your contribution" button_text="Support Us" button_url="https://www.paypal.me/ivanchromjak" blank="true" section="muted" align="center" %}

  {% include cta.html title="Support continuous development of this theme with your contribution" button_text="Support Us" button_url="https://www.paypal.me/ivanchromjak" blank="true" %}

{% else %}

  {% include cards.html id="home-right" style="" media="right" section="muted" %}

  {% include cards.html id="home-next" style="primary" align="center" section="muted" %}

  {% include instagram.html count="8" section="default" %}

{% endif %}

<!--
background-image: linear-gradient(to right, #0acffe 0%, #495aff 100%);
background-image: linear-gradient(-225deg, #AC32E4 0%, #7918F2 48%, #4801FF 100%);
background-image: linear-gradient(-225deg, #A445B2 0%, #D41872 52%, #FF0066 100%); -->

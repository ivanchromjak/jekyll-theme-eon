---
title: Contact Form
excerpt: 'Multipurpose Jekyll theme. Create company or personal site and host on GitHub for free.
          <br><br>
          <a class="uk-button uk-button-large uk-button-danger uk-box-shadow-medium hvr-up" href="https://github.com/ivanchromjak/jekyll-theme-plus/fork"><span uk-icon="github"></span> Fork on GitHub</a> &nbsp;
          <a class="uk-button uk-button-large uk-button-light uk-box-shadow-medium hvr-up" href="https://github.com/ivanchromjak/jekyll-theme-plus/fork"><span uk-icon="copy"></span> Documentation</a>'
permalink: /contact-form/
navbar:
  sticky: false
  animation: true
  transparent: true
  transparent_color: light
header:
    background_image: https://source.unsplash.com/aViOQZzikVs
    background_align: center
    background_color: "linear-gradient(-40deg, #0acffe 0%, #495aff 100%)"
    background_overlay: true
    color: dark
    align: center-
    search: true
    newsletter: mailchimp
    height: full
    image: /assets/icons/rocket-2.svg
---

{% include formspree.html email="my_name@gmail.com" redirect="/thanks/" %}

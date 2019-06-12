---
title: Contact Form
subtitle: The options and posibilities are endless
width: default
sidebar: 
  left: blog
  right: page  
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: center # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image: https://source.unsplash.com/FgSyP02I0gw/1800x700
  background_overlay: "rgba(0, 0, 0, 0.45)"
  color: light
  section_size: large
  heading_size: medium
  parallax: true
---

Example contact us form using [Formspree](https://formspree.io/).

{% include formspree.html email="my_name@gmail.com" redirect="/thanks/" name="false" subject="false" %}

{% include formspree.html email="my_name@gmail.com" redirect="/thanks/" name="true" subject="true" %}


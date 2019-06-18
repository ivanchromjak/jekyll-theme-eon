---
title: Call To Action
width: full
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: 1-1 # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_color: "#D95B72"
  section_size: large
  heading_size: large
  color: light
  parallax: true
  container:
    block: header-1
---


{% include mailchimp.html 
  section_size="large"
  section_title="Mailchimp newsletter signup"
  section_subtitle="Out of with muff safe found in yourself took didn't god, the world have the bedding hardly"
  section_container="xsmall"
  section_header_align="center"
  section_background="primary"
%}

{% include cta.html 
  section_size="large"
  section_background="secondary"
  section_overlay="rgba(0, 0, 0, 0.8)"
  section_content_color="light"
  layout="three"
  block="cta-1"
%}

{% include cta.html 
  section_size="large"
  section_image="section-2.jpeg"
  section_overlay="rgba(13, 57, 181, 0.8)"
  section_container="small"
  section_content_align="center"
  section_content_color="light"
  layout="one"
  block="cta-3"
%}

{% include cta.html 
  section_size="large"
  section_container="small"
  layout="two"
  block="cta-2"
%}
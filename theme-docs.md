---
title: Theme Docs
width: xsmall
navbar:
  sticky: true
  scroll_up: true
  animation: true
  transparent: true
  transparent_color: light
header:
  layout: center # Options: left, center, 1-1, 1-2, 1-3 or 2-3
  background_image: https://source.unsplash.com/f77Bh3inUpE/1600x700
  background_overlay: "rgba(0, 0, 0, 0.5)"
  color: light
  section_size: large
  heading_size: medium
  parallax: true
---

* TOC
{:toc}

### Site and author details
Add your site and author details in `_config.yml`:

```yaml
title:              Docs
description:        Documentation Jekyll theme.
lang:               en

# Site subpath, e.g. /blog
baseurl:            ""

# Permalink URLs structure, for permalink style options see: https://jekyllrb.com/docs/permalinks/
permalink:          /:title/

# Site base hostname & protocol, e.g. http://example.com
url:                "https://docs.jekyll.plus"

# Site logo # e.g. logo.png, upload logo image file to /uploads/ folder
logo:      

# Default author settings
author:
    name:           Pete Seth
    title:          Lead Developer  
    avatar:         avatar-tom.png
```

### Update favicon

You can find the current favicon (favicon.png) inside the theme `/uploads/` directory, just replace it with your new favicon.